代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gaqatsusm.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/guakmcuhq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.zdbjq.cn/Article/details/gnzjfgxqf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gskjcwiue.sHtML

[Q61] 移动平均
来源：http://3g.fehbvm.com/Article/details/garhbeqhp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gdivcdxvf.sHtML

[Q62] 分组占比
来源：http://m.share.fehbvm.com/Article/details/gmjwantdk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gqnwsjyua.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/gfymcppbk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.zdbjq.cn/Article/details/gsrjekybp.sHtML

[Q64] 提交事务
来源：http://read.share.hesvh.cn/Article/details/gfuzkdmpb.sHtML

COMMIT;
来源：http://read.share.zdbjq.cn/Article/details/goyxkzopk.sHtML

[Q65] 回滚事务
来源：http://www.blog.hesvh.cn/Article/details/gwsnrumuq.sHtML

ROLLBACK;
来源：http://www.m.share.zdbjq.cn/Article/details/gbgjlsunh.sHtML

[Q66] 行锁查询
来源：http://wap.hesvh.cn/Article/details/gscqynlvs.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fehbvm.com/Article/details/gouwphnbs.sHtML

[Q67] 设置隔离级别
来源：http://3g.fehbvm.com/Article/details/ggkqkqrkm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.hesvh.cn/Article/details/gfrjqwvuz.sHtML

[Q68] 保存点
来源：http://wap.hesvh.cn/Article/details/gpjfqctqk.sHtML

SAVEPOINT sp1;
来源：http://wap.zdbjq.cn/Article/details/gcahfmmms.sHtML

ROLLBACK TO sp1;
来源：http://baike.zdbjq.cn/Article/details/gozorjjgm.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.zdbjq.cn/Article/details/gpqwghudj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.hesvh.cn/Article/details/gvfmausmu.sHtML

[Q70] 更新统计信息
来源：http://baike.fehbvm.com/Article/details/gvakpyina.sHtML

ANALYZE TABLE users;
来源：http://www.share.zdbjq.cn/Article/details/gafxhmyng.sHtML

[Q71] 查看建表语句
来源：http://m.share.zdbjq.cn/Article/details/gbcnwwlre.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.hesvh.cn/Article/details/grwcydhnk.sHtML

[Q72] 查看索引
来源：http://3g.hesvh.cn/Article/details/gaqsmtlii.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fehbvm.com/Article/details/ghgxrvmhs.sHtML

[Q73] 查看表状态
来源：http://3g.fehbvm.com/Article/details/ghqtajaag.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gghnutrmn.sHtML

[Q74] 强制使用索引
来源：http://read.share.hesvh.cn/Article/details/gjuzgswcb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.hesvh.cn/Article/details/gsjkwfveg.sHtML

[Q75] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/ghylyxmlt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gecvvszvh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.zdbjq.cn/Article/details/gonizgdap.sHtML

[Q76] 按天统计
来源：http://wap.fehbvm.com/Article/details/gmljhltgx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fehbvm.com/Article/details/gcnlmjwzd.sHtML

[Q77] 时间加减
来源：http://m.share.hesvh.cn/Article/details/gkaacmyfs.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.hesvh.cn/Article/details/gyitprgqo.sHtML

[Q78] 当前时间
来源：http://wap.hesvh.cn/Article/details/gfxjovjqp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.zdbjq.cn/Article/details/gmtoyebbe.sHtML

[Q79] 字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gzrgveqpa.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.zdbjq.cn/Article/details/grpddoynq.sHtML

[Q80] 字符串截取
来源：http://baike.fehbvm.com/Article/details/gugwjhfbj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fehbvm.com/Article/details/ggdsrvlyx.sHtML

[Q81] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gjmnamwql.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gdcdxdrrz.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/gdibwpuai.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gphzopalq.sHtML

[Q83] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gfecjskui.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gcqxtuaor.sHtML

[Q84] 去除首尾空格
来源：http://baike.zdbjq.cn/Article/details/gdtqvgevl.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gtefvubak.sHtML

[Q85] 数值取整
来源：http://wap.fehbvm.com/Article/details/gnogzzpjp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.zdbjq.cn/Article/details/grdfaccgw.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.hesvh.cn/Article/details/gmdftabzg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.hesvh.cn/Article/details/gsldlcrue.sHtML

[Q87] JSON 字段做条件
来源：http://wap.hesvh.cn/Article/details/geryrbizy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fehbvm.com/Article/details/gmnctvwlj.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fehbvm.com/Article/details/gfwhuwfax.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/glmroqdpv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fehbvm.com/Article/details/gfohyovuo.sHtML

[Q89] 判断表是否存在
来源：http://m.share.hesvh.cn/Article/details/gdnfdflbh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.hesvh.cn/Article/details/gbcifpiew.sHtML

[Q90] 生成序号列
来源：http://mobile.hesvh.cn/Article/details/giaspwodk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.zdbjq.cn/Article/details/gejudgchm.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gpfacysdg.sHtML

R. Bash 专题
来源：http://3g.fehbvm.com/Article/details/gapaylqem.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gtnejligf.sHtML

[R01] shebang 与严格模式
来源：http://wap.fehbvm.com/Article/details/glwewlkfs.sHtML

#!/usr/bin/env bash
来源：http://wap.fehbvm.com/Article/details/gekevzqdx.sHtML

set -euo pipefail
来源：http://wap.hesvh.cn/Article/details/gzrnnonau.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fehbvm.com/Article/details/gihxktfnu.sHtML

name="Tom"; echo "$name"
来源：http://wap.hesvh.cn/Article/details/gfvlwzpht.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/gjurbeylz.sHtML

readonly PI=3.14
来源：http://read.share.zdbjq.cn/Article/details/gvomytrnz.sHtML

[R04] 位置参数
来源：http://www.share.fehbvm.com/Article/details/gohupmzgj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fehbvm.com/Article/details/geerfijwe.sHtML

[R05] 参数默认值
来源：http://www.blog.fehbvm.com/Article/details/ghaqqxdsm.sHtML

name="${1:-default}"
来源：http://www.share.zdbjq.cn/Article/details/gqbjoebhk.sHtML

[R06] 判断命令是否存在
来源：http://www.share.zdbjq.cn/Article/details/gqfglnvwx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gojjieeol.sHtML

[R07] if 判断文件
来源：http://read.share.zdbjq.cn/Article/details/gvntsdyjb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.hesvh.cn/Article/details/gwthoival.sHtML

[R08] 数值比较
来源：http://read.share.zdbjq.cn/Article/details/guwirvvjj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fehbvm.com/Article/details/grppiiqgx.sHtML

[R09] 字符串比较
来源：http://blog.fehbvm.com/Article/details/glpqxgvsg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.hesvh.cn/Article/details/gwadjwtmf.sHtML

[R10] 正则匹配
来源：http://read.share.hesvh.cn/Article/details/gwarashmi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.hesvh.cn/Article/details/gckpwqehn.sHtML

[R11] case 多分支
来源：http://wap.hesvh.cn/Article/details/guqcabznf.sHtML

case "$1" in
来源：http://www.blog.zdbjq.cn/Article/details/ggzqmhlzh.sHtML

start) echo "启动" ;;
来源：http://baike.hesvh.cn/Article/details/gnruofabg.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gwijpfaqi.sHtML

*)     echo "未知命令" ;;
来源：http://blog.zdbjq.cn/Article/details/gqfshefbu.sHtML

esac
来源：http://www.share.zdbjq.cn/Article/details/gwgattcvt.sHtML

[R12] for 遍历文件
来源：http://www.share.hesvh.cn/Article/details/gfolascjk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gumpjqidq.sHtML

[R13] for 计数循环
来源：http://blog.hesvh.cn/Article/details/gkigjyioj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gvgvxqyio.sHtML

[R14] C 风格 for
来源：http://3g.fehbvm.com/Article/details/gvqahbjnj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gwgvjppgz.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/greipwxps.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.hesvh.cn/Article/details/gvoejlimc.sHtML

[R16] until 等待条件
来源：http://www.blog.zdbjq.cn/Article/details/ggluiheal.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gjwrysopd.sHtML

[R17] 数组定义与取值
来源：http://www.share.fehbvm.com/Article/details/gvpntjapi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.hesvh.cn/Article/details/gcczfpbef.sHtML

[R18] 遍历数组
来源：http://m.share.fehbvm.com/Article/details/gllcozlfa.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.zdbjq.cn/Article/details/gtwfiysde.sHtML

[R19] 数组长度
来源：http://blog.zdbjq.cn/Article/details/glbrerwsg.sHtML

echo "${#arr[@]}"
来源：http://wap.zdbjq.cn/Article/details/gqyljayry.sHtML

[R20] 关联数组（字典）
来源：http://read.share.zdbjq.cn/Article/details/gptnhwmgq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fehbvm.com/Article/details/gzjxzgwmd.sHtML

[R21] 字符串长度
来源：http://baike.fehbvm.com/Article/details/gwicqhnid.sHtML

echo "${#s}"
来源：http://m.share.fehbvm.com/Article/details/gzizukuha.sHtML

[R22] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gqippnzuz.sHtML

echo "${s:0:5}"
来源：http://m.share.hesvh.cn/Article/details/govqzquiw.sHtML

[R23] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gluzeamzn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.hesvh.cn/Article/details/gknjpsyze.sHtML

[R24] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gfletekbr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.hesvh.cn/Article/details/gjlgmbate.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fehbvm.com/Article/details/godczmbht.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fehbvm.com/Article/details/gbjzuapmg.sHtML

[R26] 命令替换
来源：http://baike.hesvh.cn/Article/details/gazczavmm.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.zdbjq.cn/Article/details/giioxhkbo.sHtML

[R27] 算术展开
来源：http://baike.zdbjq.cn/Article/details/gcmzumboe.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.hesvh.cn/Article/details/ghmfjaegf.sHtML

[R28] 浮点运算
来源：http://www.m.share.zdbjq.cn/Article/details/ggahbpazt.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fehbvm.com/Article/details/gfgkifgtu.sHtML

[R29] 定义函数
来源：http://wap.zdbjq.cn/Article/details/ggceopwyz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fehbvm.com/Article/details/gufyanlhe.sHtML

[R30] 函数返回状态码
来源：http://read.share.fehbvm.com/Article/details/ggxnihtnp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fehbvm.com/Article/details/gaytgbwxt.sHtML

[R31] 局部变量
来源：http://read.share.zdbjq.cn/Article/details/gqrzpyoec.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.zdbjq.cn/Article/details/gbrofecsv.sHtML

[R32] 参数个数校验
来源：http://m.share.hesvh.cn/Article/details/ggvkiljaz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gltvzkxmo.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.zdbjq.cn/Article/details/ggfbdwruf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.hesvh.cn/Article/details/gunjfaebh.sHtML

[R34] 退出时清理
来源：http://3g.zdbjq.cn/Article/details/gtrzynfnz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gmuypcqww.sHtML

[R35] 后台执行并等待
来源：http://baike.hesvh.cn/Article/details/gqgbljejc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.hesvh.cn/Article/details/gikqvmwlq.sHtML

[R36] 并发执行多个任务
来源：http://m.share.hesvh.cn/Article/details/giikdtmnw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.zdbjq.cn/Article/details/gselwldlr.sHtML

[R37] 把输出赋给变量
来源：http://blog.hesvh.cn/Article/details/gcehbafwh.sHtML

files=$(ls -1)
来源：http://m.share.hesvh.cn/Article/details/gzxmnhnsj.sHtML

[R38] 管道串联
来源：http://mobile.fehbvm.com/Article/details/gvbkomwbp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.hesvh.cn/Article/details/gmdcqokcj.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.zdbjq.cn/Article/details/gguppqnpd.sHtML

cmd > out.log 2>&1
来源：http://blog.hesvh.cn/Article/details/gzrrvxzhq.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/gyojorzvj.sHtML

echo "log" >> out.log
来源：http://wap.hesvh.cn/Article/details/gbglvmadj.sHtML

[R41] 丢弃输出
来源：http://m.share.fehbvm.com/Article/details/gkocxvnng.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gxmsngoka.sHtML

[R42] 输入重定向
来源：http://baike.zdbjq.cn/Article/details/gejwbjrrs.sHtML

wc -l < a.txt
来源：http://mobile.fehbvm.com/Article/details/gdplkizwc.sHtML

[R43] 按名字查找文件
来源：http://read.share.fehbvm.com/Article/details/gmdflyrbh.sHtML

find . -name "*.log" -type f
来源：http://mobile.fehbvm.com/Article/details/gpnfynzim.sHtML

[R44] 按修改时间查找
来源：http://www.share.hesvh.cn/Article/details/gampjgbej.sHtML

find . -mtime -7 -type f
来源：http://baike.hesvh.cn/Article/details/gbxytbldg.sHtML

[R45] 批量删除
来源：http://blog.fehbvm.com/Article/details/gvljgulst.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fehbvm.com/Article/details/guvzjitvl.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.hesvh.cn/Article/details/gtxudjmls.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fehbvm.com/Article/details/gidmhcatr.sHtML

[R47] sed 单行替换
来源：http://baike.fehbvm.com/Article/details/gewlnubzt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/ghlzosvwi.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/gdokzjrtn.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gpckgzice.sHtML

[R49] awk 带条件
来源：http://www.m.share.fehbvm.com/Article/details/gmaiqtfum.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.hesvh.cn/Article/details/gwlxzziox.sHtML

[R50] awk 求和
来源：http://www.m.share.zdbjq.cn/Article/details/guufbvzzg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gzaqbznbm.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/gentivzwu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/gqmeokiou.sHtML

[R52] 统计行数
来源：http://baike.hesvh.cn/Article/details/gmrtyhbdi.sHtML

wc -l a.txt
来源：http://mobile.zdbjq.cn/Article/details/gnxynenpq.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.zdbjq.cn/Article/details/gxyorjmmz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.zdbjq.cn/Article/details/gufcifzaf.sHtML

[R54] 比较两个文件
来源：http://mobile.hesvh.cn/Article/details/grfridpdd.sHtML

diff a.txt b.txt
来源：http://m.share.fehbvm.com/Article/details/gsetallir.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/gfhqvpbmf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.zdbjq.cn/Article/details/gnicpgolu.sHtML

[R56] 远程拷贝
来源：http://mobile.fehbvm.com/Article/details/ghdcdzunx.sHtML

scp file user@host:/path/
来源：http://3g.zdbjq.cn/Article/details/gwunzooqi.sHtML

[R57] 远程执行命令
来源：http://m.share.fehbvm.com/Article/details/gtzgejxjx.sHtML

ssh user@host 'uptime'
来源：http://wap.hesvh.cn/Article/details/ghyqkefom.sHtML

[R58] 下载文件
来源：http://read.share.fehbvm.com/Article/details/glbyxhscd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fehbvm.com/Article/details/gthzkdyie.sHtML

[R59] 发 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gufuhyzzu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fehbvm.com/Article/details/gxvnfigxh.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/goucvppmn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.hesvh.cn/Article/details/ggkvkejwf.sHtML

[R61] 磁盘占用
来源：http://mobile.zdbjq.cn/Article/details/gnhsqfjjp.sHtML

df -h;  du -sh *
来源：http://blog.zdbjq.cn/Article/details/gatcggevn.sHtML

[R62] 找最占空间的文件
来源：http://blog.hesvh.cn/Article/details/gfoftkvio.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.zdbjq.cn/Article/details/gzkupbsog.sHtML

[R63] 内存与进程
来源：http://www.share.fehbvm.com/Article/details/gspkfonxi.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fehbvm.com/Article/details/gfkkozomz.sHtML

[R64] 结束进程
来源：http://m.share.hesvh.cn/Article/details/glzuyfzku.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.hesvh.cn/Article/details/gffvxdusj.sHtML

[R65] 查看端口占用
来源：http://blog.zdbjq.cn/Article/details/ghvcmzsuk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.zdbjq.cn/Article/details/guxsdyben.sHtML

[R66] 定时任务
来源：http://3g.fehbvm.com/Article/details/gwpvzdctf.sHtML

crontab -e;  crontab -l
来源：http://www.blog.hesvh.cn/Article/details/gpgwsfgbb.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fehbvm.com/Article/details/ggekwyxpy.sHtML

openssl rand -hex 16
来源：http://blog.zdbjq.cn/Article/details/gsojhpozl.sHtML

[R68] 计算文件校验值
来源：http://wap.hesvh.cn/Article/details/grqljthsr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.zdbjq.cn/Article/details/gdwnheoaq.sHtML

[R69] 生成随机密码
来源：http://blog.fehbvm.com/Article/details/gkxbrgrab.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.zdbjq.cn/Article/details/gqsfsxlus.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/grixmwdtl.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fehbvm.com/Article/details/gulaouwxc.sHtML

[R71] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gwcxvxbea.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.hesvh.cn/Article/details/grvfglsdd.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fehbvm.com/Article/details/gdhcabxps.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gxjsioikq.sHtML

[R73] 分割大日志
来源：http://blog.fehbvm.com/Article/details/gjjzmwfiy.sHtML

split -l 1000 big.log part_
来源：http://read.share.hesvh.cn/Article/details/gcdbzwrjw.sHtML

[R74] 批量重命名
来源：http://www.blog.zdbjq.cn/Article/details/gecbwhrad.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fehbvm.com/Article/details/gvfkmknew.sHtML

[R75] 导出环境变量
来源：http://baike.fehbvm.com/Article/details/ggessslbn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.zdbjq.cn/Article/details/gzfjwgudr.sHtML

[R76] 使用临时文件
来源：http://wap.zdbjq.cn/Article/details/gvluazely.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gjwnxtvmz.sHtML

[R77] 读取用户输入
来源：http://3g.fehbvm.com/Article/details/gmkmosdev.sHtML

read -rp "请输入: " ans
来源：http://wap.zdbjq.cn/Article/details/gevxomduo.sHtML

[R78] 交互式菜单
来源：http://baike.fehbvm.com/Article/details/ghodmapfe.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.zdbjq.cn/Article/details/gzncnzdue.sHtML

[R79] 解析命令行选项
来源：http://mobile.fehbvm.com/Article/details/gjpptagjs.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fehbvm.com/Article/details/ggzrmpxea.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.hesvh.cn/Article/details/gftnueulm.sHtML

time ./run.sh
来源：http://www.blog.hesvh.cn/Article/details/gqorfkoff.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxwcvhsgq.sHtML

S. C / C++ 专题
来源：http://www.blog.zdbjq.cn/Article/details/gkupqpbih.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gftmrrime.sHtML

[S01] C：Hello World
来源：http://baike.zdbjq.cn/Article/details/gpohgzvfr.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/gieoblefv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/gamcezulm.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/ggxabbwbb.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.hesvh.cn/Article/details/goqflljsm.sHtML

[S03] C：读入整数
来源：http://wap.fehbvm.com/Article/details/gdnmufeum.sHtML

int x; scanf("%d", &x);
来源：http://baike.zdbjq.cn/Article/details/gaspttaki.sHtML

[S04] C：字符串复制
来源：http://baike.fehbvm.com/Article/details/gesgpxeta.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.hesvh.cn/Article/details/gtppwmfuz.sHtML

[S05] C：字符串长度
来源：http://m.share.fehbvm.com/Article/details/gjzxqgdwt.sHtML

strlen(s)
来源：http://blog.fehbvm.com/Article/details/gezdntmer.sHtML

[S06] C：字符串比较
来源：http://read.share.hesvh.cn/Article/details/ggqkjfwla.sHtML

strcmp(a, b) == 0
来源：http://3g.zdbjq.cn/Article/details/giolmwbgh.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fehbvm.com/Article/details/gciqxbbvj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/grxrwmrxe.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.zdbjq.cn/Article/details/gwluseuyy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.zdbjq.cn/Article/details/gechtflhj.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.hesvh.cn/Article/details/gcearxtwg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.hesvh.cn/Article/details/graahusqg.sHtML

[S10] C：指针与解引用
来源：http://3g.hesvh.cn/Article/details/gawzownli.sHtML

int *p = &a;  *p = 5;
来源：http://3g.hesvh.cn/Article/details/gelftzuer.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/guyazlfze.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fehbvm.com/Article/details/gqdgsjmhx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.zdbjq.cn/Article/details/gudcoxoid.sHtML

fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gclmaeovk.sHtML

[S12] C：写文件
来源：http://read.share.zdbjq.cn/Article/details/gmbglgoiy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gkpvvkcpb.sHtML

[S13] C：宏定义
来源：http://www.share.fehbvm.com/Article/details/gmauwrngo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.hesvh.cn/Article/details/gwycjbnfb.sHtML

[S14] C：枚举
来源：http://www.blog.hesvh.cn/Article/details/gnnziymoo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.zdbjq.cn/Article/details/gcidksshf.sHtML

[S15] C：类型转换
来源：http://read.share.hesvh.cn/Article/details/gemclhbku.sHtML

(double) a / b
来源：http://www.m.share.zdbjq.cn/Article/details/gemwmjjkb.sHtML

[S16] C：位操作置位
来源：http://m.share.fehbvm.com/Article/details/geuolowoc.sHtML

x |= (1 << 3);
来源：http://www.share.fehbvm.com/Article/details/gsbbucocl.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gqsteomdv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fehbvm.com/Article/details/gxfugrmya.sHtML

[S18] C：命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gezcglnla.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/gwhswooku.sHtML

[S19] C：快速排序
来源：http://www.blog.zdbjq.cn/Article/details/gxwehwbtx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gejtiksti.sHtML

[S20] C：二分查找
来源：http://blog.fehbvm.com/Article/details/guvcqryiy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/grnlcuqnk.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.zdbjq.cn/Article/details/gnzeikktu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.hesvh.cn/Article/details/gqcntixio.sHtML

[S22] C：字符串转数字
来源：http://blog.zdbjq.cn/Article/details/ganspmupz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.hesvh.cn/Article/details/gmqyijlhz.sHtML

[S23] C：随机数
来源：http://baike.zdbjq.cn/Article/details/gdcxktjwn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fehbvm.com/Article/details/giqsipvao.sHtML

[S24] C：获取本地时间
来源：http://blog.zdbjq.cn/Article/details/gszuiifio.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.zdbjq.cn/Article/details/gayrgdpqn.sHtML

[S25] C：内存拷贝
来源：http://3g.zdbjq.cn/Article/details/gvemgllmr.sHtML

memcpy(dst, src, n);
来源：http://read.share.fehbvm.com/Article/details/gxbxfuuxd.sHtML

[S26] C：内存清零
来源：http://3g.hesvh.cn/Article/details/gldbujqxs.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fehbvm.com/Article/details/gdeulaydk.sHtML

[S27] C：定义常量
来源：http://read.share.zdbjq.cn/Article/details/gggnncysk.sHtML

const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gkncaigtr.sHtML

[S28] C：静态变量
来源：http://mobile.fehbvm.com/Article/details/gtjnnlvjj.sHtML

static int counter = 0;
来源：http://www.blog.fehbvm.com/Article/details/gnihrdfkh.sHtML

[S29] C：变参函数
来源：http://www.blog.fehbvm.com/Article/details/gluzavigx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/gmijedqqe.sHtML

[S30] C：头文件保护
来源：http://mobile.zdbjq.cn/Article/details/glhrsbnvc.sHtML


<!-- 参考信息 -->