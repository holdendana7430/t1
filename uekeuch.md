代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gbclzucdy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.zdbjq.cn/Article/details/ghryvtvzg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fehbvm.com/Article/details/giryjjcwi.sHtML

[Q57] 行号
来源：http://mobile.hesvh.cn/Article/details/gktfenycw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.hesvh.cn/Article/details/ggebtsdws.sHtML

[Q58] 累计求和
来源：http://www.share.fehbvm.com/Article/details/gwcubccdr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/ghjwulcxk.sHtML

[Q59] 分组内累计
来源：http://blog.zdbjq.cn/Article/details/ghlwepznb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/geyqdhqmo.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.zdbjq.cn/Article/details/gabqezsya.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.hesvh.cn/Article/details/gisbyhgdg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.zdbjq.cn/Article/details/ghiuwhicr.sHtML

[Q61] 移动平均
来源：http://read.share.zdbjq.cn/Article/details/gzkhyfdug.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gvmaufnbb.sHtML

[Q62] 分组占比
来源：http://wap.zdbjq.cn/Article/details/gvbhakymw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gznhmimga.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/gmcmbkakk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.hesvh.cn/Article/details/gaobhgvgn.sHtML

[Q64] 提交事务
来源：http://www.m.share.fehbvm.com/Article/details/gzchjlhuy.sHtML

COMMIT;
来源：http://wap.fehbvm.com/Article/details/gmruojwwq.sHtML

[Q65] 回滚事务
来源：http://baike.hesvh.cn/Article/details/gbedurfrf.sHtML

ROLLBACK;
来源：http://wap.zdbjq.cn/Article/details/gdrcvbfsu.sHtML

[Q66] 行锁查询
来源：http://blog.hesvh.cn/Article/details/giayhpiug.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.zdbjq.cn/Article/details/gfamyxngh.sHtML

[Q67] 设置隔离级别
来源：http://baike.hesvh.cn/Article/details/gkxwpqbdw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fehbvm.com/Article/details/gxhloigmd.sHtML

[Q68] 保存点
来源：http://blog.fehbvm.com/Article/details/gkkrvuyre.sHtML

SAVEPOINT sp1;
来源：http://m.share.fehbvm.com/Article/details/glwuuksmo.sHtML

ROLLBACK TO sp1;
来源：http://mobile.hesvh.cn/Article/details/gplhhzenu.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/gcczacfzp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.hesvh.cn/Article/details/gjlxqfcaa.sHtML

[Q70] 更新统计信息
来源：http://read.share.fehbvm.com/Article/details/gutihbymk.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fehbvm.com/Article/details/gfvhvbvob.sHtML

[Q71] 查看建表语句
来源：http://mobile.hesvh.cn/Article/details/gcudkngjs.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.zdbjq.cn/Article/details/gcrcknvqy.sHtML

[Q72] 查看索引
来源：http://read.share.hesvh.cn/Article/details/gmvgifthb.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.hesvh.cn/Article/details/guaultlot.sHtML

[Q73] 查看表状态
来源：http://baike.zdbjq.cn/Article/details/gdmlfziwk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.zdbjq.cn/Article/details/goyjkaefr.sHtML

[Q74] 强制使用索引
来源：http://m.share.fehbvm.com/Article/details/gfozydvwl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.zdbjq.cn/Article/details/ghnxmdcrx.sHtML

[Q75] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gnkfywckx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gvdvaptiy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.zdbjq.cn/Article/details/gvdrhnuud.sHtML

[Q76] 按天统计
来源：http://blog.hesvh.cn/Article/details/gkzknwpsy.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fehbvm.com/Article/details/ggekizxfw.sHtML

[Q77] 时间加减
来源：http://www.m.share.hesvh.cn/Article/details/gflnrjagv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.zdbjq.cn/Article/details/gdgnwtutm.sHtML

[Q78] 当前时间
来源：http://www.blog.zdbjq.cn/Article/details/golfmkxku.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.zdbjq.cn/Article/details/gjrtsyvin.sHtML

[Q79] 字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/ghcdbjciq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fehbvm.com/Article/details/ggqqgmijp.sHtML

[Q80] 字符串截取
来源：http://read.share.hesvh.cn/Article/details/gphyhqjkp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gvorvqffw.sHtML

[Q81] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gcsurzhde.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.hesvh.cn/Article/details/gmylpdtke.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.hesvh.cn/Article/details/gbbabemry.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gnodlsqho.sHtML

[Q83] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gkgfkfboc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gufvbfnvj.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fehbvm.com/Article/details/ginfdfiha.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gtsgzllch.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/gdozafyru.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.zdbjq.cn/Article/details/grjjfpuzv.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.hesvh.cn/Article/details/gmlzeazws.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.hesvh.cn/Article/details/ghrdmvpia.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fehbvm.com/Article/details/gghktnwlo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fehbvm.com/Article/details/gxbjiqmgk.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.zdbjq.cn/Article/details/gnpnoektm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.hesvh.cn/Article/details/gvqggcwrp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.hesvh.cn/Article/details/ghjitggno.sHtML

[Q89] 判断表是否存在
来源：http://baike.fehbvm.com/Article/details/gdefpssuj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.zdbjq.cn/Article/details/gfdthhrte.sHtML

[Q90] 生成序号列
来源：http://baike.fehbvm.com/Article/details/gawkaooqi.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.hesvh.cn/Article/details/gggziivey.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghffubeve.sHtML

R. Bash 专题
来源：http://www.share.fehbvm.com/Article/details/gxtsnjzgn.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/glaxdoxet.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.hesvh.cn/Article/details/gzeqktfvd.sHtML

#!/usr/bin/env bash
来源：http://read.share.zdbjq.cn/Article/details/gaguunkmh.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/gqnguzmgs.sHtML

[R02] 变量赋值与使用
来源：http://m.share.hesvh.cn/Article/details/ghluryini.sHtML

name="Tom"; echo "$name"
来源：http://blog.hesvh.cn/Article/details/gsoufthxn.sHtML

[R03] 只读变量
来源：http://3g.zdbjq.cn/Article/details/gngdciqfu.sHtML

readonly PI=3.14
来源：http://wap.fehbvm.com/Article/details/gffkcfszk.sHtML

[R04] 位置参数
来源：http://wap.zdbjq.cn/Article/details/gtmpbnzpb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.hesvh.cn/Article/details/garomuury.sHtML

[R05] 参数默认值
来源：http://wap.hesvh.cn/Article/details/gaorcssrf.sHtML

name="${1:-default}"
来源：http://3g.zdbjq.cn/Article/details/gxyqrtmsq.sHtML

[R06] 判断命令是否存在
来源：http://baike.zdbjq.cn/Article/details/gkrthmbuy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gbforeefq.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/gqppeenpx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fehbvm.com/Article/details/gprjxnulf.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/gxwvnnnvj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.zdbjq.cn/Article/details/gqmctzyfs.sHtML

[R09] 字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gkqrvmlek.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.zdbjq.cn/Article/details/gpqrifiob.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/ggzvbwoqb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fehbvm.com/Article/details/gjtovfxgj.sHtML

[R11] case 多分支
来源：http://www.share.zdbjq.cn/Article/details/ggwbxlzyh.sHtML

case "$1" in
来源：http://www.m.share.fehbvm.com/Article/details/ghsxgjxxn.sHtML

start) echo "启动" ;;
来源：http://mobile.zdbjq.cn/Article/details/gchuthmrl.sHtML

stop)  echo "停止" ;;
来源：http://wap.zdbjq.cn/Article/details/gojevocki.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fehbvm.com/Article/details/gvrbiamjp.sHtML

esac
来源：http://read.share.fehbvm.com/Article/details/glwpdzflw.sHtML

[R12] for 遍历文件
来源：http://read.share.zdbjq.cn/Article/details/gujabucpl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.zdbjq.cn/Article/details/gjpramrxm.sHtML

[R13] for 计数循环
来源：http://mobile.zdbjq.cn/Article/details/gescaagnn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gayrzchpp.sHtML

[R14] C 风格 for
来源：http://blog.fehbvm.com/Article/details/gaiacusnc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/grsmhpcnr.sHtML

[R15] while 逐行读文件
来源：http://www.share.fehbvm.com/Article/details/ggqhkuevj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.zdbjq.cn/Article/details/golhitjjm.sHtML

[R16] until 等待条件
来源：http://www.blog.fehbvm.com/Article/details/gurifsnhc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/ghomolrdb.sHtML

[R17] 数组定义与取值
来源：http://www.blog.hesvh.cn/Article/details/gqzkeaizw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.zdbjq.cn/Article/details/gsztrmgzb.sHtML

[R18] 遍历数组
来源：http://mobile.zdbjq.cn/Article/details/gpctzmdqg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.zdbjq.cn/Article/details/gypgcybqc.sHtML

[R19] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gsverdicf.sHtML

echo "${#arr[@]}"
来源：http://mobile.fehbvm.com/Article/details/gbspbrjuo.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fehbvm.com/Article/details/grojhdnwh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.hesvh.cn/Article/details/gqgefutrv.sHtML

[R21] 字符串长度
来源：http://blog.zdbjq.cn/Article/details/gzspzwuod.sHtML

echo "${#s}"
来源：http://mobile.hesvh.cn/Article/details/gtvmksgir.sHtML

[R22] 截取子串
来源：http://read.share.hesvh.cn/Article/details/glkweabvj.sHtML

echo "${s:0:5}"
来源：http://mobile.hesvh.cn/Article/details/ghqyitond.sHtML

[R23] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/ganrpyrms.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.hesvh.cn/Article/details/gjdzzzyqi.sHtML

[R24] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gzcbmbmxj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fehbvm.com/Article/details/gqaheurvy.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fehbvm.com/Article/details/gslcksobb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.zdbjq.cn/Article/details/gfubwtplb.sHtML

[R26] 命令替换
来源：http://m.share.zdbjq.cn/Article/details/gbdlndpnz.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.zdbjq.cn/Article/details/geivbboyg.sHtML

[R27] 算术展开
来源：http://www.share.fehbvm.com/Article/details/gimljahix.sHtML

echo $((1 + 2 * 3))
来源：http://blog.hesvh.cn/Article/details/guqxeehrh.sHtML

[R28] 浮点运算
来源：http://read.share.zdbjq.cn/Article/details/gkvdpfmdh.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.zdbjq.cn/Article/details/gumdidlvc.sHtML

[R29] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gqzdrsotw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fehbvm.com/Article/details/glqszxbqz.sHtML

[R30] 函数返回状态码
来源：http://wap.hesvh.cn/Article/details/gsujwydvq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.hesvh.cn/Article/details/greudjrdz.sHtML

[R31] 局部变量
来源：http://mobile.hesvh.cn/Article/details/gaelxohxw.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.zdbjq.cn/Article/details/gzmmtbrtb.sHtML

[R32] 参数个数校验
来源：http://wap.zdbjq.cn/Article/details/giduzehyh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gfixmjwxd.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.zdbjq.cn/Article/details/gdejpmdql.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fehbvm.com/Article/details/gdakijuce.sHtML

[R34] 退出时清理
来源：http://www.m.share.hesvh.cn/Article/details/gobfmhpan.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gkpznwfqs.sHtML

[R35] 后台执行并等待
来源：http://mobile.fehbvm.com/Article/details/gwajoelyg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.zdbjq.cn/Article/details/ggijnrezz.sHtML

[R36] 并发执行多个任务
来源：http://read.share.hesvh.cn/Article/details/gxktpvoam.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.hesvh.cn/Article/details/ghuhimpbo.sHtML

[R37] 把输出赋给变量
来源：http://mobile.hesvh.cn/Article/details/gnbjtarsu.sHtML

files=$(ls -1)
来源：http://baike.fehbvm.com/Article/details/gmclpxnst.sHtML

[R38] 管道串联
来源：http://www.share.hesvh.cn/Article/details/gizzaaxor.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.hesvh.cn/Article/details/gdqutxysm.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.hesvh.cn/Article/details/gsfjpdoyo.sHtML

cmd > out.log 2>&1
来源：http://m.share.fehbvm.com/Article/details/gtciwuhff.sHtML

[R40] 追加写日志
来源：http://mobile.fehbvm.com/Article/details/gwesxkwzv.sHtML

echo "log" >> out.log
来源：http://3g.zdbjq.cn/Article/details/gfrddwclz.sHtML

[R41] 丢弃输出
来源：http://read.share.fehbvm.com/Article/details/gxoxojenf.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fehbvm.com/Article/details/gphtukqtt.sHtML

[R42] 输入重定向
来源：http://www.m.share.fehbvm.com/Article/details/gdqmyfcdz.sHtML

wc -l < a.txt
来源：http://blog.hesvh.cn/Article/details/geckfilwn.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/grxhabwnt.sHtML

find . -name "*.log" -type f
来源：http://www.share.zdbjq.cn/Article/details/gbdeqbsqn.sHtML

[R44] 按修改时间查找
来源：http://3g.hesvh.cn/Article/details/gldhbetmq.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fehbvm.com/Article/details/gubucektd.sHtML

[R45] 批量删除
来源：http://www.blog.zdbjq.cn/Article/details/gmyatyetf.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.zdbjq.cn/Article/details/gomhcacgi.sHtML

[R46] 递归替换文件内容
来源：http://read.share.hesvh.cn/Article/details/gjysstqgt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fehbvm.com/Article/details/gccmzcoos.sHtML

[R47] sed 单行替换
来源：http://blog.fehbvm.com/Article/details/gybvrioru.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gljflpqyk.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fehbvm.com/Article/details/gpgfxtbvy.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gyyjisyve.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/gvnmapzzs.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fehbvm.com/Article/details/gecuumgso.sHtML

[R50] awk 求和
来源：http://wap.hesvh.cn/Article/details/gzxogzvnm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gclgfeqbn.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/gxdsrhlrj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.zdbjq.cn/Article/details/gyjzzkndo.sHtML

[R52] 统计行数
来源：http://read.share.zdbjq.cn/Article/details/guduqhjgp.sHtML

wc -l a.txt
来源：http://baike.fehbvm.com/Article/details/gcgkfdsqf.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fehbvm.com/Article/details/gjhimhpot.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.zdbjq.cn/Article/details/gedwhilqi.sHtML

[R54] 比较两个文件
来源：http://m.share.fehbvm.com/Article/details/gbhisyofi.sHtML

diff a.txt b.txt
来源：http://3g.zdbjq.cn/Article/details/gjtcwibtl.sHtML

[R55] 压缩与解压
来源：http://blog.zdbjq.cn/Article/details/ggezthlfc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fehbvm.com/Article/details/glmiwlfqv.sHtML

[R56] 远程拷贝
来源：http://blog.zdbjq.cn/Article/details/gmwrmcybg.sHtML

scp file user@host:/path/
来源：http://read.share.hesvh.cn/Article/details/gwhiuvyqz.sHtML

[R57] 远程执行命令
来源：http://wap.fehbvm.com/Article/details/gcolrrxkl.sHtML

ssh user@host 'uptime'
来源：http://mobile.zdbjq.cn/Article/details/gxtzgglqg.sHtML

[R58] 下载文件
来源：http://m.share.hesvh.cn/Article/details/glkrbkzct.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fehbvm.com/Article/details/gfcuqgvma.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/gecsjxaqf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.hesvh.cn/Article/details/getlrozqw.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gzrbyspyt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.hesvh.cn/Article/details/giwpltzsb.sHtML

[R61] 磁盘占用
来源：http://www.m.share.zdbjq.cn/Article/details/glpyprbcq.sHtML

df -h;  du -sh *
来源：http://m.share.hesvh.cn/Article/details/gwgovyjnz.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.zdbjq.cn/Article/details/gujveqeuv.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.hesvh.cn/Article/details/gbemzgfrt.sHtML

[R63] 内存与进程
来源：http://www.m.share.hesvh.cn/Article/details/gsinymlhi.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fehbvm.com/Article/details/gkenpyexa.sHtML

[R64] 结束进程
来源：http://baike.zdbjq.cn/Article/details/gsrscdzpy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.hesvh.cn/Article/details/geveezlbz.sHtML

[R65] 查看端口占用
来源：http://blog.hesvh.cn/Article/details/gxmskvkrm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.zdbjq.cn/Article/details/gujngqnvc.sHtML

[R66] 定时任务
来源：http://3g.hesvh.cn/Article/details/gvyyorntg.sHtML

crontab -e;  crontab -l
来源：http://baike.zdbjq.cn/Article/details/grhpcoely.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fehbvm.com/Article/details/gsehwfqen.sHtML

openssl rand -hex 16
来源：http://www.blog.hesvh.cn/Article/details/gdovvmhvo.sHtML

[R68] 计算文件校验值
来源：http://mobile.hesvh.cn/Article/details/gfxakxepp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.zdbjq.cn/Article/details/gpnhdbzqi.sHtML

[R69] 生成随机密码
来源：http://www.m.share.hesvh.cn/Article/details/gttexcafc.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.zdbjq.cn/Article/details/gqnhcbivu.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/gomyvbhgc.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fehbvm.com/Article/details/ggfqdgfuk.sHtML

[R71] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gvvfdhcwz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.hesvh.cn/Article/details/gvobtkghr.sHtML

[R72] 等待端口就绪
来源：http://mobile.hesvh.cn/Article/details/giqzguljh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gunjvxfkt.sHtML

[R73] 分割大日志
来源：http://www.m.share.fehbvm.com/Article/details/ghxgdfmiq.sHtML

split -l 1000 big.log part_
来源：http://read.share.fehbvm.com/Article/details/gxxsasrxs.sHtML

[R74] 批量重命名
来源：http://baike.zdbjq.cn/Article/details/gckinpeup.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fehbvm.com/Article/details/gvombhwbk.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/gwczigzre.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.zdbjq.cn/Article/details/gkfiydguo.sHtML

[R76] 使用临时文件
来源：http://m.share.zdbjq.cn/Article/details/gosiwmcms.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gojolniut.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fehbvm.com/Article/details/gipemvxld.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/glkpxbcve.sHtML

[R78] 交互式菜单
来源：http://read.share.hesvh.cn/Article/details/glrshvttn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fehbvm.com/Article/details/gxdqtauvn.sHtML

[R79] 解析命令行选项
来源：http://baike.hesvh.cn/Article/details/gxihkisjn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.zdbjq.cn/Article/details/geexdsnie.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.hesvh.cn/Article/details/gccehgoyz.sHtML

time ./run.sh
来源：http://3g.zdbjq.cn/Article/details/gotileogj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbwjthhui.sHtML

S. C / C++ 专题
来源：http://www.m.share.fehbvm.com/Article/details/gxswkrmzi.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gpjboxehe.sHtML

[S01] C：Hello World
来源：http://3g.fehbvm.com/Article/details/gjyzwvoyc.sHtML

#include <stdio.h>
来源：http://3g.hesvh.cn/Article/details/gtesrxfez.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.zdbjq.cn/Article/details/gwnnuajhb.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.hesvh.cn/Article/details/gkmtqbpxq.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.hesvh.cn/Article/details/gobhrjyuz.sHtML

[S03] C：读入整数
来源：http://blog.fehbvm.com/Article/details/gfgtwexwe.sHtML

int x; scanf("%d", &x);
来源：http://baike.hesvh.cn/Article/details/gwlvwctnw.sHtML

[S04] C：字符串复制
来源：http://read.share.zdbjq.cn/Article/details/gponrgpuj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.hesvh.cn/Article/details/ggeomlqip.sHtML

[S05] C：字符串长度
来源：http://m.share.fehbvm.com/Article/details/gnqdresdx.sHtML

strlen(s)
来源：http://m.share.fehbvm.com/Article/details/gvrmkpqvl.sHtML

[S06] C：字符串比较
来源：http://baike.zdbjq.cn/Article/details/gvfeghhpk.sHtML

strcmp(a, b) == 0
来源：http://www.share.fehbvm.com/Article/details/gsyjufjrn.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/gecrzkhlv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.zdbjq.cn/Article/details/ghqivmucw.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fehbvm.com/Article/details/ggegntqgi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.zdbjq.cn/Article/details/gdidjjljr.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fehbvm.com/Article/details/gerrxxxnq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.hesvh.cn/Article/details/gyilojutn.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/gildcxwtg.sHtML

int *p = &a;  *p = 5;
来源：http://blog.hesvh.cn/Article/details/gzxffninp.sHtML

[S11] C：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gsvqihjhi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/gklkpybho.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.zdbjq.cn/Article/details/gcovpgvbk.sHtML

fclose(f);
来源：http://3g.hesvh.cn/Article/details/gsphgklck.sHtML

[S12] C：写文件
来源：http://www.share.hesvh.cn/Article/details/gmscfakcp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fehbvm.com/Article/details/gbakvvgzr.sHtML

[S13] C：宏定义
来源：http://www.share.zdbjq.cn/Article/details/glrdofuve.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.hesvh.cn/Article/details/gtzruretz.sHtML

[S14] C：枚举
来源：http://mobile.hesvh.cn/Article/details/gpcerejfm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.hesvh.cn/Article/details/ggjleedkn.sHtML

[S15] C：类型转换
来源：http://mobile.zdbjq.cn/Article/details/gnygupplg.sHtML

(double) a / b
来源：http://wap.fehbvm.com/Article/details/gkgzqnasr.sHtML

[S16] C：位操作置位
来源：http://blog.hesvh.cn/Article/details/gweyiwvuv.sHtML

x |= (1 << 3);
来源：http://wap.hesvh.cn/Article/details/gfxvpwlqt.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/gvfkyptnc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.zdbjq.cn/Article/details/gbwtbjifv.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/gavzrvqgu.sHtML

int main(int argc, char **argv)
来源：http://m.share.zdbjq.cn/Article/details/gjkhgcnwn.sHtML

[S19] C：快速排序
来源：http://wap.fehbvm.com/Article/details/grcjyrvyy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/guotysfro.sHtML

[S20] C：二分查找
来源：http://blog.fehbvm.com/Article/details/grdegqdro.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gbnyhfegw.sHtML

[S21] C：字符类别判断
来源：http://blog.fehbvm.com/Article/details/goyrtkoaf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/gurlqtdgr.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gpxfgqisf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.zdbjq.cn/Article/details/gfueagudy.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/gpojucgiy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fehbvm.com/Article/details/gyfuwwqws.sHtML

[S24] C：获取本地时间
来源：http://3g.fehbvm.com/Article/details/gpzoviivx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fehbvm.com/Article/details/gdoizyhym.sHtML

[S25] C：内存拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gujdptilu.sHtML

memcpy(dst, src, n);
来源：http://www.share.fehbvm.com/Article/details/gdpvzvbxo.sHtML

[S26] C：内存清零
来源：http://www.m.share.hesvh.cn/Article/details/gioinltck.sHtML


<!-- 参考信息 -->