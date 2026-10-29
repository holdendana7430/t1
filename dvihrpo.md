代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gavipxwkd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.hesvh.cn/Article/details/gjmustrez.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gotmdlotg.sHtML

[Q57] 行号
来源：http://www.share.hesvh.cn/Article/details/gzpjnrmra.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.hesvh.cn/Article/details/gzzhfvcis.sHtML

[Q58] 累计求和
来源：http://www.share.zdbjq.cn/Article/details/gdopperpy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gsxmziyrn.sHtML

[Q59] 分组内累计
来源：http://www.share.zdbjq.cn/Article/details/gvjeaqrab.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gebojpltw.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fehbvm.com/Article/details/gplfxzcvj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fehbvm.com/Article/details/gkyxtsgxx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.hesvh.cn/Article/details/geltvxgxg.sHtML

[Q61] 移动平均
来源：http://www.m.share.fehbvm.com/Article/details/guhmlarke.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/glxdmvqru.sHtML

[Q62] 分组占比
来源：http://www.blog.hesvh.cn/Article/details/ghxivpwet.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gzlyqzufm.sHtML

[Q63] 开启事务
来源：http://wap.fehbvm.com/Article/details/ghghseiqk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fehbvm.com/Article/details/gbuitfkgp.sHtML

[Q64] 提交事务
来源：http://3g.zdbjq.cn/Article/details/gbuzbklrv.sHtML

COMMIT;
来源：http://m.share.fehbvm.com/Article/details/gtshbtnwa.sHtML

[Q65] 回滚事务
来源：http://read.share.hesvh.cn/Article/details/gyryoypow.sHtML

ROLLBACK;
来源：http://blog.zdbjq.cn/Article/details/gtaeppebj.sHtML

[Q66] 行锁查询
来源：http://blog.hesvh.cn/Article/details/gcawqskwx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.zdbjq.cn/Article/details/gsqtadury.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fehbvm.com/Article/details/grvofsuud.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.zdbjq.cn/Article/details/giqznfxbn.sHtML

[Q68] 保存点
来源：http://wap.zdbjq.cn/Article/details/gfisgpugb.sHtML

SAVEPOINT sp1;
来源：http://www.share.zdbjq.cn/Article/details/gmqmpphwu.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fehbvm.com/Article/details/gpwfejntw.sHtML

[Q69] 查看执行计划
来源：http://m.share.hesvh.cn/Article/details/gboitrrda.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fehbvm.com/Article/details/gfdvxdksl.sHtML

[Q70] 更新统计信息
来源：http://m.share.fehbvm.com/Article/details/gxzwatrsb.sHtML

ANALYZE TABLE users;
来源：http://m.share.hesvh.cn/Article/details/gcuevswgb.sHtML

[Q71] 查看建表语句
来源：http://mobile.zdbjq.cn/Article/details/gkwxnyzhf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.hesvh.cn/Article/details/gokqdiuui.sHtML

[Q72] 查看索引
来源：http://www.blog.fehbvm.com/Article/details/guojsgipu.sHtML

SHOW INDEX FROM users;
来源：http://m.share.hesvh.cn/Article/details/gstxssufy.sHtML

[Q73] 查看表状态
来源：http://blog.fehbvm.com/Article/details/gnbfigpcu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.zdbjq.cn/Article/details/ghbwfqgbk.sHtML

[Q74] 强制使用索引
来源：http://read.share.fehbvm.com/Article/details/gkkpnvimv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.hesvh.cn/Article/details/gpvpoqkoc.sHtML

[Q75] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gzbcjanav.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gmomxqsxy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.zdbjq.cn/Article/details/gpehibxnq.sHtML

[Q76] 按天统计
来源：http://read.share.hesvh.cn/Article/details/gixawyvmf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.hesvh.cn/Article/details/gtotakyfe.sHtML

[Q77] 时间加减
来源：http://mobile.zdbjq.cn/Article/details/gepzoxvty.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fehbvm.com/Article/details/gnalzuxeb.sHtML

[Q78] 当前时间
来源：http://m.share.hesvh.cn/Article/details/grsdmfopv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.hesvh.cn/Article/details/gbpnfuyzh.sHtML

[Q79] 字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gjkeeeqiq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.zdbjq.cn/Article/details/gjftcoiqu.sHtML

[Q80] 字符串截取
来源：http://blog.hesvh.cn/Article/details/gofmmqhct.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.zdbjq.cn/Article/details/ggvlkhsso.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gfuaexmuo.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fehbvm.com/Article/details/gjmyblmzs.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fehbvm.com/Article/details/gvvzzuwrs.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gnonyrtwu.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gunfzyxlr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/giklztijr.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.hesvh.cn/Article/details/gnhprtvzg.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gxdjqzjsd.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/gsnnjrdgm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fehbvm.com/Article/details/gpixjtapg.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.zdbjq.cn/Article/details/genracain.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fehbvm.com/Article/details/gnjmhbdbw.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.hesvh.cn/Article/details/gsivrrxml.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fehbvm.com/Article/details/gkekwwxbf.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.hesvh.cn/Article/details/gwdvnkboh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.zdbjq.cn/Article/details/gancbghau.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.zdbjq.cn/Article/details/gdzsyppik.sHtML

[Q89] 判断表是否存在
来源：http://3g.zdbjq.cn/Article/details/glnjnuvfh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.hesvh.cn/Article/details/gtwazfsqq.sHtML

[Q90] 生成序号列
来源：http://www.blog.fehbvm.com/Article/details/ggqexhfyu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fehbvm.com/Article/details/gdbjkifjw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gsumzoryj.sHtML

R. Bash 专题
来源：http://www.m.share.hesvh.cn/Article/details/gjbuucttd.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gcfzfjlml.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.zdbjq.cn/Article/details/gacnphbie.sHtML

#!/usr/bin/env bash
来源：http://www.share.fehbvm.com/Article/details/gvfriaidp.sHtML

set -euo pipefail
来源：http://blog.hesvh.cn/Article/details/grsmjbrfn.sHtML

[R02] 变量赋值与使用
来源：http://wap.zdbjq.cn/Article/details/goytqchmi.sHtML

name="Tom"; echo "$name"
来源：http://www.share.zdbjq.cn/Article/details/grknkbwkg.sHtML

[R03] 只读变量
来源：http://m.share.hesvh.cn/Article/details/gwwaaparn.sHtML

readonly PI=3.14
来源：http://www.m.share.fehbvm.com/Article/details/gtjeayusc.sHtML

[R04] 位置参数
来源：http://read.share.fehbvm.com/Article/details/gwvqdyogh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fehbvm.com/Article/details/gddolranh.sHtML

[R05] 参数默认值
来源：http://baike.fehbvm.com/Article/details/guffakgac.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/gnfucchfy.sHtML

[R06] 判断命令是否存在
来源：http://www.share.hesvh.cn/Article/details/gdthjzsis.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/gcnzfxvil.sHtML

[R07] if 判断文件
来源：http://www.share.fehbvm.com/Article/details/ggwiukwqa.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fehbvm.com/Article/details/gcnrmiohi.sHtML

[R08] 数值比较
来源：http://www.blog.fehbvm.com/Article/details/gzyvhuuzi.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fehbvm.com/Article/details/gsqwmirxt.sHtML

[R09] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gtmhkmlbe.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fehbvm.com/Article/details/gvdaiicrw.sHtML

[R10] 正则匹配
来源：http://blog.zdbjq.cn/Article/details/gtmltgymy.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.hesvh.cn/Article/details/giskgmaud.sHtML

[R11] case 多分支
来源：http://wap.hesvh.cn/Article/details/gxtsontzy.sHtML

case "$1" in
来源：http://www.share.fehbvm.com/Article/details/gdlezokeb.sHtML

start) echo "启动" ;;
来源：http://baike.zdbjq.cn/Article/details/gadwweick.sHtML

stop)  echo "停止" ;;
来源：http://m.share.zdbjq.cn/Article/details/gwahbpekp.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.zdbjq.cn/Article/details/gxanmvxqj.sHtML

esac
来源：http://www.m.share.fehbvm.com/Article/details/glnwobjhg.sHtML

[R12] for 遍历文件
来源：http://baike.zdbjq.cn/Article/details/ghahqjxzd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fehbvm.com/Article/details/gcmuvscpt.sHtML

[R13] for 计数循环
来源：http://read.share.fehbvm.com/Article/details/ghekpvrag.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gdbprvqne.sHtML

[R14] C 风格 for
来源：http://3g.fehbvm.com/Article/details/gtvqdnynb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/grnmtwgsp.sHtML

[R15] while 逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/guiaiodjr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.hesvh.cn/Article/details/gfgnatmql.sHtML

[R16] until 等待条件
来源：http://mobile.zdbjq.cn/Article/details/gkrnmuxxr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gaojbagen.sHtML

[R17] 数组定义与取值
来源：http://wap.zdbjq.cn/Article/details/guxfpwjnu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.hesvh.cn/Article/details/gagqlytaf.sHtML

[R18] 遍历数组
来源：http://3g.zdbjq.cn/Article/details/gikvizugs.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fehbvm.com/Article/details/goagugjtk.sHtML

[R19] 数组长度
来源：http://wap.fehbvm.com/Article/details/gljqzxvum.sHtML

echo "${#arr[@]}"
来源：http://m.share.hesvh.cn/Article/details/gdbeynqdb.sHtML

[R20] 关联数组（字典）
来源：http://wap.fehbvm.com/Article/details/gazcnfuff.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fehbvm.com/Article/details/gknviewmd.sHtML

[R21] 字符串长度
来源：http://blog.zdbjq.cn/Article/details/gjuesdvpt.sHtML

echo "${#s}"
来源：http://mobile.hesvh.cn/Article/details/gmtbbuqul.sHtML

[R22] 截取子串
来源：http://mobile.fehbvm.com/Article/details/guseygslh.sHtML

echo "${s:0:5}"
来源：http://www.share.fehbvm.com/Article/details/gkyepoyyt.sHtML

[R23] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/ggaiuhnnv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.hesvh.cn/Article/details/ggobceudl.sHtML

[R24] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gjqcudnid.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fehbvm.com/Article/details/grewumoqn.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/gfhbckmga.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.zdbjq.cn/Article/details/ggtcyimel.sHtML

[R26] 命令替换
来源：http://baike.zdbjq.cn/Article/details/gxzvecmxg.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fehbvm.com/Article/details/gwedyahdk.sHtML

[R27] 算术展开
来源：http://www.m.share.fehbvm.com/Article/details/gnqijxehp.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.zdbjq.cn/Article/details/gusehkcsy.sHtML

[R28] 浮点运算
来源：http://wap.fehbvm.com/Article/details/ginvhezuv.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/grmyqncwo.sHtML

[R29] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gxheapttw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/gopuuubrl.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fehbvm.com/Article/details/gkeiiyuxp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/gryvzaerf.sHtML

[R31] 局部变量
来源：http://3g.zdbjq.cn/Article/details/gjmdpsxzx.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fehbvm.com/Article/details/gxxrcbjcv.sHtML

[R32] 参数个数校验
来源：http://3g.hesvh.cn/Article/details/ghhncambj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gdltrukhi.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.zdbjq.cn/Article/details/gaycikjmx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/gqliotgkv.sHtML

[R34] 退出时清理
来源：http://3g.fehbvm.com/Article/details/gdhsqgmol.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gmvrfwatf.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fehbvm.com/Article/details/grjxpyugh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.hesvh.cn/Article/details/gdrhmqiyg.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fehbvm.com/Article/details/gjgnirwty.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.hesvh.cn/Article/details/goauoyafl.sHtML

[R37] 把输出赋给变量
来源：http://wap.hesvh.cn/Article/details/gnsvxzfvf.sHtML

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/gsvpdufhv.sHtML

[R38] 管道串联
来源：http://www.blog.fehbvm.com/Article/details/gdnxgmobg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fehbvm.com/Article/details/gmfdsomub.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.hesvh.cn/Article/details/gmjlarcny.sHtML

cmd > out.log 2>&1
来源：http://baike.hesvh.cn/Article/details/gcpkidoxy.sHtML

[R40] 追加写日志
来源：http://baike.hesvh.cn/Article/details/gdwtaxxxt.sHtML

echo "log" >> out.log
来源：http://baike.fehbvm.com/Article/details/gjkaasbdv.sHtML

[R41] 丢弃输出
来源：http://wap.zdbjq.cn/Article/details/gmjugarry.sHtML

cmd >/dev/null 2>&1
来源：http://wap.hesvh.cn/Article/details/gtjspcixp.sHtML

[R42] 输入重定向
来源：http://mobile.fehbvm.com/Article/details/gyaxqfbud.sHtML

wc -l < a.txt
来源：http://www.share.hesvh.cn/Article/details/gauireial.sHtML

[R43] 按名字查找文件
来源：http://mobile.zdbjq.cn/Article/details/gbtocqaly.sHtML

find . -name "*.log" -type f
来源：http://baike.zdbjq.cn/Article/details/gkorhoqtl.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/ghfvwvdux.sHtML

find . -mtime -7 -type f
来源：http://wap.hesvh.cn/Article/details/gfjkyiddd.sHtML

[R45] 批量删除
来源：http://www.blog.hesvh.cn/Article/details/gcfcowaus.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.zdbjq.cn/Article/details/ggclicgff.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fehbvm.com/Article/details/gstnsuetp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/gjfunjwhw.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fehbvm.com/Article/details/ggtkgnyed.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fehbvm.com/Article/details/gepfjloma.sHtML

[R48] awk 取指定列
来源：http://blog.zdbjq.cn/Article/details/gdmxkibpl.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gcuspdxeo.sHtML

[R49] awk 带条件
来源：http://www.blog.zdbjq.cn/Article/details/ghvqfwhla.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/gswvglnvn.sHtML

[R50] awk 求和
来源：http://read.share.fehbvm.com/Article/details/gnlpygcps.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/gusfamswo.sHtML

[R51] 排序去重取前几
来源：http://www.blog.hesvh.cn/Article/details/ghcgttmyz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.zdbjq.cn/Article/details/gqieyeuqx.sHtML

[R52] 统计行数
来源：http://read.share.zdbjq.cn/Article/details/gkeztoqdm.sHtML

wc -l a.txt
来源：http://3g.fehbvm.com/Article/details/ggqdtghkx.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.zdbjq.cn/Article/details/gpafuzmcl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.zdbjq.cn/Article/details/gzktflnhf.sHtML

[R54] 比较两个文件
来源：http://blog.zdbjq.cn/Article/details/gfowxxtuz.sHtML

diff a.txt b.txt
来源：http://3g.zdbjq.cn/Article/details/glpydnxbx.sHtML

[R55] 压缩与解压
来源：http://www.blog.fehbvm.com/Article/details/gdysqivky.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.hesvh.cn/Article/details/gmhmqijxw.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/gpzsqdead.sHtML

scp file user@host:/path/
来源：http://wap.fehbvm.com/Article/details/ghbzgjyoq.sHtML

[R57] 远程执行命令
来源：http://blog.zdbjq.cn/Article/details/gayjuwsiw.sHtML

ssh user@host 'uptime'
来源：http://mobile.fehbvm.com/Article/details/gimxoxxxh.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/gmgndbbfm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.zdbjq.cn/Article/details/gvvnqefjs.sHtML

[R59] 发 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/glmpzwmux.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.hesvh.cn/Article/details/gbscczpjo.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gqayjqcdg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.zdbjq.cn/Article/details/ghurfdtdn.sHtML

[R61] 磁盘占用
来源：http://blog.zdbjq.cn/Article/details/gcnzhqmln.sHtML

df -h;  du -sh *
来源：http://read.share.zdbjq.cn/Article/details/gxlgeyekl.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fehbvm.com/Article/details/gksqlsxvf.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fehbvm.com/Article/details/gzduhikqe.sHtML

[R63] 内存与进程
来源：http://read.share.zdbjq.cn/Article/details/gmgekejrj.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.zdbjq.cn/Article/details/gzcckyxdj.sHtML

[R64] 结束进程
来源：http://www.m.share.fehbvm.com/Article/details/gambevfra.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.zdbjq.cn/Article/details/gorohwsxi.sHtML

[R65] 查看端口占用
来源：http://www.share.zdbjq.cn/Article/details/gvwbdtjsp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fehbvm.com/Article/details/gpqjvjyvy.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/gdowkqhua.sHtML

crontab -e;  crontab -l
来源：http://3g.zdbjq.cn/Article/details/goalvdomv.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fehbvm.com/Article/details/gjxxxavzu.sHtML

openssl rand -hex 16
来源：http://baike.hesvh.cn/Article/details/gedjqivwq.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.zdbjq.cn/Article/details/gpnpoocvn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gbylsvgbt.sHtML

[R69] 生成随机密码
来源：http://www.m.share.hesvh.cn/Article/details/gtldwbxie.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.zdbjq.cn/Article/details/ghjjpqcsb.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/gjaiouacv.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fehbvm.com/Article/details/ghulwrfpl.sHtML

[R71] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gsqphlbqy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/gutkchkxo.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/gnxzzidcq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gluigaoun.sHtML

[R73] 分割大日志
来源：http://www.blog.hesvh.cn/Article/details/gbhevigcu.sHtML

split -l 1000 big.log part_
来源：http://3g.fehbvm.com/Article/details/gkonghiut.sHtML

[R74] 批量重命名
来源：http://blog.hesvh.cn/Article/details/gtrbdwgme.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.hesvh.cn/Article/details/ghwwgbzeu.sHtML

[R75] 导出环境变量
来源：http://wap.zdbjq.cn/Article/details/grvopugng.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fehbvm.com/Article/details/gjuxtuzzu.sHtML

[R76] 使用临时文件
来源：http://wap.hesvh.cn/Article/details/gmsjkincv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gsvtdsujn.sHtML

[R77] 读取用户输入
来源：http://m.share.fehbvm.com/Article/details/gbqafizdj.sHtML

read -rp "请输入: " ans
来源：http://m.share.fehbvm.com/Article/details/ghsfdzekf.sHtML

[R78] 交互式菜单
来源：http://baike.zdbjq.cn/Article/details/gesccpgfa.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/gnooymili.sHtML

[R79] 解析命令行选项
来源：http://read.share.zdbjq.cn/Article/details/gcitcmbku.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.hesvh.cn/Article/details/gdurbkufd.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.hesvh.cn/Article/details/ghwedtrhq.sHtML

time ./run.sh
来源：http://baike.hesvh.cn/Article/details/gwyirkubp.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gppuhqbjd.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/gdfexjsim.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjizrqndh.sHtML

[S01] C：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gegoefhxl.sHtML

#include <stdio.h>
来源：http://wap.fehbvm.com/Article/details/gkakurngd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fehbvm.com/Article/details/gndiqjdmw.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/gxgqlaxgw.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fehbvm.com/Article/details/gwkfljhkz.sHtML

[S03] C：读入整数
来源：http://blog.hesvh.cn/Article/details/ggtkpfdda.sHtML

int x; scanf("%d", &x);
来源：http://3g.zdbjq.cn/Article/details/gtszxqwpy.sHtML

[S04] C：字符串复制
来源：http://baike.fehbvm.com/Article/details/gbxahtjdz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.hesvh.cn/Article/details/gsqugygiv.sHtML

[S05] C：字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gvdsunmbu.sHtML

strlen(s)
来源：http://www.m.share.hesvh.cn/Article/details/gbrtzklbo.sHtML

[S06] C：字符串比较
来源：http://wap.zdbjq.cn/Article/details/gbigvbiuw.sHtML

strcmp(a, b) == 0
来源：http://m.share.zdbjq.cn/Article/details/gquzssxne.sHtML

[S07] C：数组遍历求和
来源：http://blog.zdbjq.cn/Article/details/gafszfskv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/gzcjhdsra.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fehbvm.com/Article/details/geoyeltia.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/ggrozevzf.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.hesvh.cn/Article/details/gewvpnvhr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fehbvm.com/Article/details/ganczczyw.sHtML

[S10] C：指针与解引用
来源：http://blog.hesvh.cn/Article/details/gdpccryfc.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.zdbjq.cn/Article/details/gtcvodkoa.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gjztzwvtd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/ggtfonheu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fehbvm.com/Article/details/gwjzzfdvv.sHtML

fclose(f);
来源：http://3g.zdbjq.cn/Article/details/guwevidaw.sHtML

[S12] C：写文件
来源：http://blog.fehbvm.com/Article/details/gghgcaazy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/goefvdsfo.sHtML

[S13] C：宏定义
来源：http://m.share.zdbjq.cn/Article/details/gzsjuhlxu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/gfynyhzuh.sHtML

[S14] C：枚举
来源：http://wap.hesvh.cn/Article/details/gadvuynse.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.hesvh.cn/Article/details/gnmwhjbte.sHtML

[S15] C：类型转换
来源：http://3g.zdbjq.cn/Article/details/gluaeswlp.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/grbiefurq.sHtML

[S16] C：位操作置位
来源：http://wap.zdbjq.cn/Article/details/gitblqzuf.sHtML

x |= (1 << 3);
来源：http://blog.fehbvm.com/Article/details/gwdpvajid.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gnrslyuoo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.hesvh.cn/Article/details/gaggnmpfe.sHtML

[S18] C：命令行参数
来源：http://m.share.hesvh.cn/Article/details/gbjxmxttr.sHtML

int main(int argc, char **argv)
来源：http://mobile.hesvh.cn/Article/details/gemmajusc.sHtML

[S19] C：快速排序
来源：http://blog.fehbvm.com/Article/details/gvihnuzoh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/ggnwnbokp.sHtML

[S20] C：二分查找
来源：http://www.m.share.hesvh.cn/Article/details/gotjtjehi.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/grrjvypvq.sHtML

[S21] C：字符类别判断
来源：http://3g.zdbjq.cn/Article/details/gamsxazug.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.hesvh.cn/Article/details/gfqijtntw.sHtML

[S22] C：字符串转数字
来源：http://blog.hesvh.cn/Article/details/giijadfcr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/gxzqmrflo.sHtML

[S23] C：随机数
来源：http://www.m.share.fehbvm.com/Article/details/gdveqivxk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/grfgrakgb.sHtML

[S24] C：获取本地时间
来源：http://3g.zdbjq.cn/Article/details/gurbuapyb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/gapwroxua.sHtML

[S25] C：内存拷贝
来源：http://baike.hesvh.cn/Article/details/gaqfmfwyf.sHtML

memcpy(dst, src, n);
来源：http://m.share.hesvh.cn/Article/details/gpnrctenx.sHtML

[S26] C：内存清零
来源：http://blog.fehbvm.com/Article/details/gwmksjqoe.sHtML


<!-- 参考信息 -->