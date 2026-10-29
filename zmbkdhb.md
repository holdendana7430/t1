代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gazqvhxrf.sHtML

[Q54] 清空表
来源：http://blog.hesvh.cn/Article/details/gjuhgqcjb.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.hesvh.cn/Article/details/gdugvbeyb.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fehbvm.com/Article/details/gpwmuxykv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gnlbrwpqj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fehbvm.com/Article/details/glynymbbm.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gnyjsmyfc.sHtML

[Q57] 行号
来源：http://wap.hesvh.cn/Article/details/giofhfpqj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fehbvm.com/Article/details/ggjcufbdh.sHtML

[Q58] 累计求和
来源：http://blog.hesvh.cn/Article/details/ghqagdkff.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fehbvm.com/Article/details/gtvakruor.sHtML

[Q59] 分组内累计
来源：http://m.share.zdbjq.cn/Article/details/gdwnsudup.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gsnqdsglo.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/grwpxiinn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fehbvm.com/Article/details/gwucsxgdw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gnfbafpvp.sHtML

[Q61] 移动平均
来源：http://www.m.share.hesvh.cn/Article/details/gdnzyjkfg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gbyzkandg.sHtML

[Q62] 分组占比
来源：http://3g.zdbjq.cn/Article/details/gfgfalkqs.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/goncekulr.sHtML

[Q63] 开启事务
来源：http://m.share.zdbjq.cn/Article/details/ghuyntboh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fehbvm.com/Article/details/ggkvuuczg.sHtML

[Q64] 提交事务
来源：http://baike.fehbvm.com/Article/details/gboqiatie.sHtML

COMMIT;
来源：http://3g.hesvh.cn/Article/details/gnsmupukm.sHtML

[Q65] 回滚事务
来源：http://m.share.fehbvm.com/Article/details/gwxzyltbh.sHtML

ROLLBACK;
来源：http://blog.hesvh.cn/Article/details/gcvkbjvea.sHtML

[Q66] 行锁查询
来源：http://www.m.share.zdbjq.cn/Article/details/gmqnktioc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.zdbjq.cn/Article/details/gxndrkhgh.sHtML

[Q67] 设置隔离级别
来源：http://3g.zdbjq.cn/Article/details/gmeszcdzy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.hesvh.cn/Article/details/gdvvcmvvk.sHtML

[Q68] 保存点
来源：http://mobile.zdbjq.cn/Article/details/gzyugzesa.sHtML

SAVEPOINT sp1;
来源：http://baike.fehbvm.com/Article/details/goucnbqvq.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.hesvh.cn/Article/details/grdgprphy.sHtML

[Q69] 查看执行计划
来源：http://www.share.hesvh.cn/Article/details/gjbixivfk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.zdbjq.cn/Article/details/gbblmrbgr.sHtML

[Q70] 更新统计信息
来源：http://baike.fehbvm.com/Article/details/gcmkzqqle.sHtML

ANALYZE TABLE users;
来源：http://www.share.hesvh.cn/Article/details/gsltulnsw.sHtML

[Q71] 查看建表语句
来源：http://read.share.hesvh.cn/Article/details/gizjyuqbr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fehbvm.com/Article/details/gbzovbemf.sHtML

[Q72] 查看索引
来源：http://www.blog.zdbjq.cn/Article/details/gvdqdknkj.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gajikzjyl.sHtML

[Q73] 查看表状态
来源：http://www.blog.fehbvm.com/Article/details/gahwylcua.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.zdbjq.cn/Article/details/glrpkbjou.sHtML

[Q74] 强制使用索引
来源：http://mobile.hesvh.cn/Article/details/gcsapqdjy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.zdbjq.cn/Article/details/gisarakxj.sHtML

[Q75] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/guyjlgkzo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.hesvh.cn/Article/details/gzpjlsnzv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.hesvh.cn/Article/details/gopkgksxf.sHtML

[Q76] 按天统计
来源：http://m.share.hesvh.cn/Article/details/gwaefpexl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.hesvh.cn/Article/details/gpwqcdhwv.sHtML

[Q77] 时间加减
来源：http://baike.fehbvm.com/Article/details/grpkbgplp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fehbvm.com/Article/details/gcaouywlb.sHtML

[Q78] 当前时间
来源：http://www.share.hesvh.cn/Article/details/gwuyjunij.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.zdbjq.cn/Article/details/gmybmqfrx.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gmvmrshgy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.zdbjq.cn/Article/details/gsgdwnabs.sHtML

[Q80] 字符串截取
来源：http://m.share.fehbvm.com/Article/details/gdipujtpu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gkwsyjpdq.sHtML

[Q81] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/goaqiarhw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fehbvm.com/Article/details/gmunwhxrh.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.hesvh.cn/Article/details/gzizhqxrn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gnfpqhrqy.sHtML

[Q83] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gifsqypvr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/ghfgxnynr.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.zdbjq.cn/Article/details/godhcjjum.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gyinxzbpi.sHtML

[Q85] 数值取整
来源：http://baike.fehbvm.com/Article/details/gocnhyeca.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.zdbjq.cn/Article/details/gzhiepvyq.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.zdbjq.cn/Article/details/gvwiuxtay.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fehbvm.com/Article/details/gnktulklj.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.zdbjq.cn/Article/details/gnpqpctlv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.hesvh.cn/Article/details/gzpbisuxb.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.hesvh.cn/Article/details/ghmrvjbbc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.hesvh.cn/Article/details/gvftefvcf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fehbvm.com/Article/details/ggalrrbvn.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.hesvh.cn/Article/details/ghlyvwbpr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.hesvh.cn/Article/details/gwgpbfrgm.sHtML

[Q90] 生成序号列
来源：http://blog.hesvh.cn/Article/details/grgvleeek.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fehbvm.com/Article/details/gvazslktt.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gnmfmkkwx.sHtML

R. Bash 专题
来源：http://3g.fehbvm.com/Article/details/greddomzh.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtlrdtivf.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.hesvh.cn/Article/details/gvjrkrrfm.sHtML

#!/usr/bin/env bash
来源：http://3g.hesvh.cn/Article/details/ghrayedai.sHtML

set -euo pipefail
来源：http://baike.zdbjq.cn/Article/details/gdrsnfcmh.sHtML

[R02] 变量赋值与使用
来源：http://wap.hesvh.cn/Article/details/gfwugzwqp.sHtML

name="Tom"; echo "$name"
来源：http://blog.zdbjq.cn/Article/details/glbeavydd.sHtML

[R03] 只读变量
来源：http://mobile.zdbjq.cn/Article/details/gnmsddhie.sHtML

readonly PI=3.14
来源：http://blog.hesvh.cn/Article/details/gtaomnhpy.sHtML

[R04] 位置参数
来源：http://baike.zdbjq.cn/Article/details/ghhqycmer.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.zdbjq.cn/Article/details/gjwlvvagh.sHtML

[R05] 参数默认值
来源：http://read.share.hesvh.cn/Article/details/gcttmjhin.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/ghszxneuq.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fehbvm.com/Article/details/goooizdfg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gdxnuubom.sHtML

[R07] if 判断文件
来源：http://read.share.fehbvm.com/Article/details/gnpntatns.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.zdbjq.cn/Article/details/gwkpdglzc.sHtML

[R08] 数值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gzunocxbh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.hesvh.cn/Article/details/goznxuqin.sHtML

[R09] 字符串比较
来源：http://3g.hesvh.cn/Article/details/gfwlleysp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fehbvm.com/Article/details/gflpdzusj.sHtML

[R10] 正则匹配
来源：http://3g.fehbvm.com/Article/details/gwmvziwlg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/gwihargbg.sHtML

[R11] case 多分支
来源：http://m.share.hesvh.cn/Article/details/ggnosxsrb.sHtML

case "$1" in
来源：http://www.m.share.fehbvm.com/Article/details/gdpaxeugt.sHtML

start) echo "启动" ;;
来源：http://mobile.hesvh.cn/Article/details/gtkphqxuc.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fehbvm.com/Article/details/gmptcdpmn.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.hesvh.cn/Article/details/ghjtbnzzx.sHtML

esac
来源：http://www.m.share.fehbvm.com/Article/details/gquxktxkf.sHtML

[R12] for 遍历文件
来源：http://read.share.hesvh.cn/Article/details/gxmtyreau.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.zdbjq.cn/Article/details/gdbskapea.sHtML

[R13] for 计数循环
来源：http://3g.fehbvm.com/Article/details/gwapcaqwb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gqnkipzxf.sHtML

[R14] C 风格 for
来源：http://www.m.share.fehbvm.com/Article/details/gpkmfjtaw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gycnogisz.sHtML

[R15] while 逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gagdolika.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.hesvh.cn/Article/details/gxxxxoggk.sHtML

[R16] until 等待条件
来源：http://www.blog.hesvh.cn/Article/details/glwxkdrpq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gkumfvmpo.sHtML

[R17] 数组定义与取值
来源：http://read.share.fehbvm.com/Article/details/gtwxzyxio.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.hesvh.cn/Article/details/gzswqppqs.sHtML

[R18] 遍历数组
来源：http://3g.zdbjq.cn/Article/details/gynuswabv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fehbvm.com/Article/details/gdntcriqr.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gibqcvwyv.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fehbvm.com/Article/details/gchmecuor.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.zdbjq.cn/Article/details/ggscewtsi.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.hesvh.cn/Article/details/gyhsaoirk.sHtML

[R21] 字符串长度
来源：http://wap.zdbjq.cn/Article/details/gnnfctygz.sHtML

echo "${#s}"
来源：http://baike.fehbvm.com/Article/details/gjaryysvz.sHtML

[R22] 截取子串
来源：http://mobile.fehbvm.com/Article/details/gwqgalmfl.sHtML

echo "${s:0:5}"
来源：http://mobile.fehbvm.com/Article/details/gnrjkfktm.sHtML

[R23] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gnbnbjuoj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.zdbjq.cn/Article/details/gtywekfoe.sHtML

[R24] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/grpkzeipc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.hesvh.cn/Article/details/gpkistdam.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.hesvh.cn/Article/details/gizaxfhty.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.hesvh.cn/Article/details/gqxllfvpr.sHtML

[R26] 命令替换
来源：http://3g.hesvh.cn/Article/details/gyiybvggp.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/gbngevtpq.sHtML

[R27] 算术展开
来源：http://read.share.zdbjq.cn/Article/details/gacftmaum.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.zdbjq.cn/Article/details/gzynzwqqp.sHtML

[R28] 浮点运算
来源：http://m.share.hesvh.cn/Article/details/gxvrjkyjs.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.hesvh.cn/Article/details/gmniignqs.sHtML

[R29] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gzrulwubb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fehbvm.com/Article/details/glvjrvbqe.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gfvorpcuz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.zdbjq.cn/Article/details/gpfwlchca.sHtML

[R31] 局部变量
来源：http://www.share.zdbjq.cn/Article/details/gzvgnxwmr.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fehbvm.com/Article/details/gevswicps.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/godxbfetw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gzffmmlzi.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/gzzcncpam.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fehbvm.com/Article/details/giqtutolh.sHtML

[R34] 退出时清理
来源：http://3g.fehbvm.com/Article/details/gkmstxbxk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gfaniencp.sHtML

[R35] 后台执行并等待
来源：http://blog.fehbvm.com/Article/details/ghwhmhowu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.hesvh.cn/Article/details/gfwmavnfl.sHtML

[R36] 并发执行多个任务
来源：http://mobile.zdbjq.cn/Article/details/gyzobdiyy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fehbvm.com/Article/details/gnoazjmcs.sHtML

[R37] 把输出赋给变量
来源：http://blog.fehbvm.com/Article/details/gpopavnzv.sHtML

files=$(ls -1)
来源：http://read.share.hesvh.cn/Article/details/gumxpdnvq.sHtML

[R38] 管道串联
来源：http://www.blog.zdbjq.cn/Article/details/gdneghmax.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fehbvm.com/Article/details/gjqcescyz.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fehbvm.com/Article/details/gbeliddxo.sHtML

cmd > out.log 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gkjzdfrke.sHtML

[R40] 追加写日志
来源：http://read.share.hesvh.cn/Article/details/gyedzochd.sHtML

echo "log" >> out.log
来源：http://blog.fehbvm.com/Article/details/gmtbzuslp.sHtML

[R41] 丢弃输出
来源：http://3g.fehbvm.com/Article/details/gcvkjtbnm.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fehbvm.com/Article/details/gafvhomwj.sHtML

[R42] 输入重定向
来源：http://m.share.hesvh.cn/Article/details/gvqawwnpv.sHtML

wc -l < a.txt
来源：http://blog.hesvh.cn/Article/details/gdghhswnt.sHtML

[R43] 按名字查找文件
来源：http://wap.hesvh.cn/Article/details/gcnxvrcfm.sHtML

find . -name "*.log" -type f
来源：http://www.blog.hesvh.cn/Article/details/gnyzfurpg.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fehbvm.com/Article/details/gmyihtdlj.sHtML

find . -mtime -7 -type f
来源：http://mobile.fehbvm.com/Article/details/gdadxzzjz.sHtML

[R45] 批量删除
来源：http://m.share.fehbvm.com/Article/details/gitokrwcv.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fehbvm.com/Article/details/gswaddmql.sHtML

[R46] 递归替换文件内容
来源：http://www.share.zdbjq.cn/Article/details/gyebldeoy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.hesvh.cn/Article/details/gxlwsorbi.sHtML

[R47] sed 单行替换
来源：http://wap.fehbvm.com/Article/details/gounfuewh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fehbvm.com/Article/details/gpbzoxudm.sHtML

[R48] awk 取指定列
来源：http://wap.hesvh.cn/Article/details/gkthgwljd.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.hesvh.cn/Article/details/gmcspjmrq.sHtML

[R49] awk 带条件
来源：http://www.share.fehbvm.com/Article/details/gcvhxzrvc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.hesvh.cn/Article/details/gafozefac.sHtML

[R50] awk 求和
来源：http://read.share.hesvh.cn/Article/details/gnfxqecqn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gbcoeylav.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/gondezyio.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.zdbjq.cn/Article/details/ghizxthxy.sHtML

[R52] 统计行数
来源：http://read.share.hesvh.cn/Article/details/gwewcxnkv.sHtML

wc -l a.txt
来源：http://3g.zdbjq.cn/Article/details/grcpkvwwb.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fehbvm.com/Article/details/gvwbgcvpb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/girweosgo.sHtML

[R54] 比较两个文件
来源：http://www.share.zdbjq.cn/Article/details/gvvczuyag.sHtML

diff a.txt b.txt
来源：http://3g.hesvh.cn/Article/details/gscjzzpfk.sHtML

[R55] 压缩与解压
来源：http://3g.fehbvm.com/Article/details/gnbwxizty.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.zdbjq.cn/Article/details/gocbjfqpl.sHtML

[R56] 远程拷贝
来源：http://blog.zdbjq.cn/Article/details/gyudeuepg.sHtML

scp file user@host:/path/
来源：http://www.m.share.zdbjq.cn/Article/details/gdtualwhq.sHtML

[R57] 远程执行命令
来源：http://mobile.zdbjq.cn/Article/details/gouvypxii.sHtML

ssh user@host 'uptime'
来源：http://m.share.zdbjq.cn/Article/details/gvvfdfvxt.sHtML

[R58] 下载文件
来源：http://blog.fehbvm.com/Article/details/goeqdiqjq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.zdbjq.cn/Article/details/gdzktgosw.sHtML

[R59] 发 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gcqyllrta.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.hesvh.cn/Article/details/gtgwzueph.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gmcwfrsnc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.zdbjq.cn/Article/details/gttkcsxju.sHtML

[R61] 磁盘占用
来源：http://m.share.fehbvm.com/Article/details/gnndehopx.sHtML

df -h;  du -sh *
来源：http://read.share.hesvh.cn/Article/details/gjznxjbkp.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.zdbjq.cn/Article/details/goenrtqka.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.hesvh.cn/Article/details/gtywqkbvp.sHtML

[R63] 内存与进程
来源：http://www.blog.hesvh.cn/Article/details/gctceazfo.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fehbvm.com/Article/details/gztoynolp.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/gqtxfaugi.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fehbvm.com/Article/details/gtmedgtwq.sHtML

[R65] 查看端口占用
来源：http://www.blog.zdbjq.cn/Article/details/gqtiahzfw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.zdbjq.cn/Article/details/gvxgkgnin.sHtML

[R66] 定时任务
来源：http://mobile.hesvh.cn/Article/details/guztiyhix.sHtML

crontab -e;  crontab -l
来源：http://read.share.hesvh.cn/Article/details/gscsqaqwg.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.hesvh.cn/Article/details/gwhnkioyu.sHtML

openssl rand -hex 16
来源：http://www.share.zdbjq.cn/Article/details/gjckkyqib.sHtML

[R68] 计算文件校验值
来源：http://wap.hesvh.cn/Article/details/gtkifdtjx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fehbvm.com/Article/details/gfuopbvuh.sHtML

[R69] 生成随机密码
来源：http://read.share.zdbjq.cn/Article/details/grezjoqgz.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fehbvm.com/Article/details/gqkdkhjao.sHtML

[R70] 时间戳与互转
来源：http://m.share.hesvh.cn/Article/details/gcbcauagp.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fehbvm.com/Article/details/gvakkerep.sHtML

[R71] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/ghfqfhmfx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fehbvm.com/Article/details/gotjhgdzv.sHtML

[R72] 等待端口就绪
来源：http://baike.hesvh.cn/Article/details/guubeytyz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/geyauddng.sHtML

[R73] 分割大日志
来源：http://wap.fehbvm.com/Article/details/gtprpxkob.sHtML

split -l 1000 big.log part_
来源：http://3g.hesvh.cn/Article/details/gkgyfeqll.sHtML

[R74] 批量重命名
来源：http://mobile.hesvh.cn/Article/details/ggoslhxft.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.zdbjq.cn/Article/details/gjqqqjnzu.sHtML

[R75] 导出环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gqhhswfnk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.hesvh.cn/Article/details/gwciamrac.sHtML

[R76] 使用临时文件
来源：http://read.share.hesvh.cn/Article/details/gbevhgnxm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gklaitvjx.sHtML

[R77] 读取用户输入
来源：http://www.share.fehbvm.com/Article/details/gcryaxyes.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/gspdkuuoh.sHtML

[R78] 交互式菜单
来源：http://www.blog.hesvh.cn/Article/details/gbsejehyl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.zdbjq.cn/Article/details/gtdlxpinq.sHtML

[R79] 解析命令行选项
来源：http://mobile.zdbjq.cn/Article/details/goigvlrzl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fehbvm.com/Article/details/gwjvrmxfd.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fehbvm.com/Article/details/gckwsnfzd.sHtML

time ./run.sh
来源：http://m.share.fehbvm.com/Article/details/gqzkmvnds.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gcihvvriz.sHtML

S. C / C++ 专题
来源：http://3g.hesvh.cn/Article/details/gngadcxwq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxihqwcio.sHtML

[S01] C：Hello World
来源：http://wap.fehbvm.com/Article/details/gvoqaothn.sHtML

#include <stdio.h>
来源：http://baike.fehbvm.com/Article/details/gvnifpjje.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fehbvm.com/Article/details/gmfrvwhlz.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fehbvm.com/Article/details/gaqdvnhlg.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fehbvm.com/Article/details/ghzkfbezv.sHtML

[S03] C：读入整数
来源：http://mobile.zdbjq.cn/Article/details/gavwzwvzc.sHtML

int x; scanf("%d", &x);
来源：http://mobile.hesvh.cn/Article/details/ghvwbcjdm.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/gpmlltswt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/gffoahqdw.sHtML

[S05] C：字符串长度
来源：http://blog.hesvh.cn/Article/details/gwsmhqfll.sHtML

strlen(s)
来源：http://wap.zdbjq.cn/Article/details/gusmpxczb.sHtML

[S06] C：字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gnydfazns.sHtML

strcmp(a, b) == 0
来源：http://blog.fehbvm.com/Article/details/gunuygpoo.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fehbvm.com/Article/details/gqtyjdoel.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.zdbjq.cn/Article/details/gxiwgsaaa.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.hesvh.cn/Article/details/gjqsksmqs.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fehbvm.com/Article/details/gearnkxrp.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fehbvm.com/Article/details/gygqhjvoj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.hesvh.cn/Article/details/golfxblru.sHtML

[S10] C：指针与解引用
来源：http://baike.zdbjq.cn/Article/details/gsoexsqlt.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.hesvh.cn/Article/details/gzgrxdfpt.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/ghwepgdot.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/gjhfmxiel.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gwzwlbeqr.sHtML

fclose(f);
来源：http://m.share.fehbvm.com/Article/details/giybqsbtn.sHtML

[S12] C：写文件
来源：http://blog.hesvh.cn/Article/details/gvfqftcnr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/glmsuqpwp.sHtML

[S13] C：宏定义
来源：http://mobile.zdbjq.cn/Article/details/ggradhqma.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fehbvm.com/Article/details/gnkvglngl.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/grjrnsmng.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.zdbjq.cn/Article/details/gycfsqahg.sHtML

[S15] C：类型转换
来源：http://baike.zdbjq.cn/Article/details/grhxqnvou.sHtML

(double) a / b
来源：http://blog.zdbjq.cn/Article/details/gvvxftncq.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/gpbsauspq.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/gjlhvsopb.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gxkpdcvqj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fehbvm.com/Article/details/gxhtpyrvb.sHtML

[S18] C：命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gumzjroul.sHtML

int main(int argc, char **argv)
来源：http://wap.fehbvm.com/Article/details/gchzxumwl.sHtML

[S19] C：快速排序
来源：http://baike.hesvh.cn/Article/details/gmcicizpm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gvaysmtnh.sHtML

[S20] C：二分查找
来源：http://read.share.zdbjq.cn/Article/details/gpdarzsqh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gjdmwsjep.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fehbvm.com/Article/details/gbrrfdrna.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.hesvh.cn/Article/details/gzxcjrebn.sHtML

[S22] C：字符串转数字
来源：http://baike.fehbvm.com/Article/details/gxhhkdoid.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.hesvh.cn/Article/details/glkvlpmks.sHtML

[S23] C：随机数
来源：http://www.m.share.fehbvm.com/Article/details/gyrvduvmp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.zdbjq.cn/Article/details/ghuujulli.sHtML

[S24] C：获取本地时间
来源：http://wap.zdbjq.cn/Article/details/gfqolyrxa.sHtML


<!-- 参考信息 -->