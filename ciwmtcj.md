代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fehbvm.com/Article/details/ghiyehlbk.sHtML

[Q54] 清空表
来源：http://3g.hesvh.cn/Article/details/gcxrmcusv.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.hesvh.cn/Article/details/gfgupbdgk.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fehbvm.com/Article/details/gyjndtsop.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.hesvh.cn/Article/details/gcxolrnua.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fehbvm.com/Article/details/ggylikojj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gmeyqugya.sHtML

[Q57] 行号
来源：http://wap.hesvh.cn/Article/details/gyloolipk.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fehbvm.com/Article/details/gxysvdlad.sHtML

[Q58] 累计求和
来源：http://www.blog.hesvh.cn/Article/details/gasomfygx.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.hesvh.cn/Article/details/gpxgdxhyc.sHtML

[Q59] 分组内累计
来源：http://wap.hesvh.cn/Article/details/gwmijhryr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gdyxraopb.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.hesvh.cn/Article/details/gbmpkrilz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.hesvh.cn/Article/details/gnlovleqr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fehbvm.com/Article/details/gwszhmjmz.sHtML

[Q61] 移动平均
来源：http://www.blog.zdbjq.cn/Article/details/ghyglmrep.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/glkvxgxsw.sHtML

[Q62] 分组占比
来源：http://baike.zdbjq.cn/Article/details/gfhdxdevo.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/ggzekzvnz.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/gzuduebwd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.hesvh.cn/Article/details/gtwrhvenj.sHtML

[Q64] 提交事务
来源：http://www.m.share.hesvh.cn/Article/details/gfawxbukg.sHtML

COMMIT;
来源：http://mobile.hesvh.cn/Article/details/gsyzrsdhh.sHtML

[Q65] 回滚事务
来源：http://3g.fehbvm.com/Article/details/gwokvokfd.sHtML

ROLLBACK;
来源：http://www.share.hesvh.cn/Article/details/gtphmoahg.sHtML

[Q66] 行锁查询
来源：http://baike.fehbvm.com/Article/details/gdlfwlqag.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fehbvm.com/Article/details/gfkyhvbgt.sHtML

[Q67] 设置隔离级别
来源：http://3g.fehbvm.com/Article/details/gyywygejh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.hesvh.cn/Article/details/gqwkccdjk.sHtML

[Q68] 保存点
来源：http://3g.fehbvm.com/Article/details/guridcvex.sHtML

SAVEPOINT sp1;
来源：http://www.share.zdbjq.cn/Article/details/gzsnsqozn.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fehbvm.com/Article/details/gcecjhxsn.sHtML

[Q69] 查看执行计划
来源：http://www.share.zdbjq.cn/Article/details/gblbhvhlu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.zdbjq.cn/Article/details/goeyyheje.sHtML

[Q70] 更新统计信息
来源：http://mobile.fehbvm.com/Article/details/gduppbzuj.sHtML

ANALYZE TABLE users;
来源：http://blog.fehbvm.com/Article/details/ggtcikggv.sHtML

[Q71] 查看建表语句
来源：http://wap.zdbjq.cn/Article/details/ghwketadl.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fehbvm.com/Article/details/ghjdyzyvh.sHtML

[Q72] 查看索引
来源：http://m.share.fehbvm.com/Article/details/glyclqrej.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fehbvm.com/Article/details/ggxxbdbex.sHtML

[Q73] 查看表状态
来源：http://3g.hesvh.cn/Article/details/gfqudmzbq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.zdbjq.cn/Article/details/gkjqtfhjj.sHtML

[Q74] 强制使用索引
来源：http://www.share.fehbvm.com/Article/details/guzfekngs.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.zdbjq.cn/Article/details/gmkmaicua.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gugrdrfxc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gwfpqdfim.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fehbvm.com/Article/details/gishwtsuz.sHtML

[Q76] 按天统计
来源：http://mobile.fehbvm.com/Article/details/gbfxgshkq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.hesvh.cn/Article/details/goyliwwph.sHtML

[Q77] 时间加减
来源：http://blog.zdbjq.cn/Article/details/gthmnosht.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.zdbjq.cn/Article/details/gisirczey.sHtML

[Q78] 当前时间
来源：http://wap.fehbvm.com/Article/details/gdwfulmpq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fehbvm.com/Article/details/gglvjoeff.sHtML

[Q79] 字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/glwlzuycs.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.zdbjq.cn/Article/details/gqxabhoja.sHtML

[Q80] 字符串截取
来源：http://3g.hesvh.cn/Article/details/girqkzytx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.zdbjq.cn/Article/details/geyyiseji.sHtML

[Q81] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gjjlxfmrn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.zdbjq.cn/Article/details/gmrnmegsn.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fehbvm.com/Article/details/gweanczsk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gcngswhuf.sHtML

[Q83] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gaqrgnadw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gusgswizq.sHtML

[Q84] 去除首尾空格
来源：http://3g.fehbvm.com/Article/details/gwcwecyli.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/ggonfeimq.sHtML

[Q85] 数值取整
来源：http://read.share.fehbvm.com/Article/details/gcglxeeaq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.hesvh.cn/Article/details/goxzrkxot.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.zdbjq.cn/Article/details/gkdtgtrns.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fehbvm.com/Article/details/ginjvmrxj.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.hesvh.cn/Article/details/grpqbzonx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.hesvh.cn/Article/details/gbuxweors.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.zdbjq.cn/Article/details/gkvegakri.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.zdbjq.cn/Article/details/gnvgcrdpg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/galvuzpti.sHtML

[Q89] 判断表是否存在
来源：http://baike.fehbvm.com/Article/details/gdlaovpfp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.hesvh.cn/Article/details/gxwlxvshc.sHtML

[Q90] 生成序号列
来源：http://www.m.share.hesvh.cn/Article/details/gelimulfw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.zdbjq.cn/Article/details/ghdqhklww.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gljizbmcm.sHtML

R. Bash 专题
来源：http://blog.hesvh.cn/Article/details/gtyvprmhh.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gtwolfvvc.sHtML

[R01] shebang 与严格模式
来源：http://www.share.zdbjq.cn/Article/details/gabxhanst.sHtML

#!/usr/bin/env bash
来源：http://read.share.fehbvm.com/Article/details/gorwrbuqr.sHtML

set -euo pipefail
来源：http://www.share.fehbvm.com/Article/details/gxgublnyt.sHtML

[R02] 变量赋值与使用
来源：http://m.share.zdbjq.cn/Article/details/giigiuhgj.sHtML

name="Tom"; echo "$name"
来源：http://www.share.zdbjq.cn/Article/details/gzpmbkqok.sHtML

[R03] 只读变量
来源：http://www.blog.fehbvm.com/Article/details/gqfzyezkb.sHtML

readonly PI=3.14
来源：http://3g.hesvh.cn/Article/details/gstdelnoe.sHtML

[R04] 位置参数
来源：http://www.m.share.hesvh.cn/Article/details/gwnliyvzs.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.hesvh.cn/Article/details/gevvrepwp.sHtML

[R05] 参数默认值
来源：http://www.blog.fehbvm.com/Article/details/gyuvudsga.sHtML

name="${1:-default}"
来源：http://blog.hesvh.cn/Article/details/gsxfgsdnv.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gpxgcvumd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gftpxyqnj.sHtML

[R07] if 判断文件
来源：http://wap.zdbjq.cn/Article/details/gjbzifuxq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fehbvm.com/Article/details/gyochlssn.sHtML

[R08] 数值比较
来源：http://blog.fehbvm.com/Article/details/golykvaab.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/gswsoepun.sHtML

[R09] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/gqlgqqlgc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.zdbjq.cn/Article/details/gxwtlwcgh.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gskafkblr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.hesvh.cn/Article/details/gyrsznndt.sHtML

[R11] case 多分支
来源：http://wap.hesvh.cn/Article/details/gjrjqogii.sHtML

case "$1" in
来源：http://3g.fehbvm.com/Article/details/gzlmhbord.sHtML

start) echo "启动" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gnqtmgbem.sHtML

stop)  echo "停止" ;;
来源：http://baike.hesvh.cn/Article/details/gbhykqhfp.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fehbvm.com/Article/details/gtwewxnoz.sHtML

esac
来源：http://read.share.fehbvm.com/Article/details/grqukdshh.sHtML

[R12] for 遍历文件
来源：http://www.m.share.hesvh.cn/Article/details/gfizvxriq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.hesvh.cn/Article/details/gpnnsmxlp.sHtML

[R13] for 计数循环
来源：http://wap.fehbvm.com/Article/details/gvhbccata.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gailcxgmi.sHtML

[R14] C 风格 for
来源：http://blog.zdbjq.cn/Article/details/giywsljlc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/girdwwets.sHtML

[R15] while 逐行读文件
来源：http://www.share.hesvh.cn/Article/details/ghegsflyv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fehbvm.com/Article/details/gjoehweqr.sHtML

[R16] until 等待条件
来源：http://wap.hesvh.cn/Article/details/gzbhtrjgz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gtpkfjsgk.sHtML

[R17] 数组定义与取值
来源：http://m.share.zdbjq.cn/Article/details/guovrmszq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fehbvm.com/Article/details/gndsfiqwy.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/gojfvjtsk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.zdbjq.cn/Article/details/gazfjappy.sHtML

[R19] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/gcbfpslct.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.hesvh.cn/Article/details/glnmrwzxg.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fehbvm.com/Article/details/gvtxumolr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.hesvh.cn/Article/details/gudfjyvdl.sHtML

[R21] 字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gahnmpgkd.sHtML

echo "${#s}"
来源：http://baike.zdbjq.cn/Article/details/gowleyoya.sHtML

[R22] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/ghnzylhow.sHtML

echo "${s:0:5}"
来源：http://www.share.zdbjq.cn/Article/details/gewgmrzuj.sHtML

[R23] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gsankgurz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.zdbjq.cn/Article/details/gyqrjdpvf.sHtML

[R24] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/guwcixoxr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fehbvm.com/Article/details/gzlrrfirw.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/giuquxmsb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fehbvm.com/Article/details/golkxclmg.sHtML

[R26] 命令替换
来源：http://www.blog.zdbjq.cn/Article/details/gkhubdcsj.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.hesvh.cn/Article/details/gneomwlbc.sHtML

[R27] 算术展开
来源：http://www.m.share.fehbvm.com/Article/details/gqjsxyvry.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.hesvh.cn/Article/details/gqosigkdf.sHtML

[R28] 浮点运算
来源：http://3g.fehbvm.com/Article/details/gefwkqvkb.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.zdbjq.cn/Article/details/gzpsiafrn.sHtML

[R29] 定义函数
来源：http://m.share.zdbjq.cn/Article/details/gpofkrrek.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.zdbjq.cn/Article/details/gmreiepvs.sHtML

[R30] 函数返回状态码
来源：http://blog.fehbvm.com/Article/details/gawsemctm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.hesvh.cn/Article/details/gpldgnvzy.sHtML

[R31] 局部变量
来源：http://wap.zdbjq.cn/Article/details/gmwyjfgei.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fehbvm.com/Article/details/gvvkenjzs.sHtML

[R32] 参数个数校验
来源：http://blog.hesvh.cn/Article/details/goifxntsm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/giuvmqajn.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.hesvh.cn/Article/details/gyxrnzaxy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.zdbjq.cn/Article/details/greowffox.sHtML

[R34] 退出时清理
来源：http://www.blog.hesvh.cn/Article/details/gxvrvxvoy.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gjwxcurmh.sHtML

[R35] 后台执行并等待
来源：http://read.share.fehbvm.com/Article/details/gzkrrwwob.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.hesvh.cn/Article/details/gfklsrsuu.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.zdbjq.cn/Article/details/gakoetiys.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fehbvm.com/Article/details/gcgedeuqq.sHtML

[R37] 把输出赋给变量
来源：http://baike.hesvh.cn/Article/details/goraiqlml.sHtML

files=$(ls -1)
来源：http://www.share.hesvh.cn/Article/details/gtobhzxyw.sHtML

[R38] 管道串联
来源：http://www.blog.hesvh.cn/Article/details/gxnygtmzy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fehbvm.com/Article/details/gruewdesn.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.hesvh.cn/Article/details/gfoqvmhkp.sHtML

cmd > out.log 2>&1
来源：http://blog.fehbvm.com/Article/details/gollqnbha.sHtML

[R40] 追加写日志
来源：http://www.m.share.zdbjq.cn/Article/details/gnpxrarbz.sHtML

echo "log" >> out.log
来源：http://3g.hesvh.cn/Article/details/gwpoyvbcg.sHtML

[R41] 丢弃输出
来源：http://www.m.share.zdbjq.cn/Article/details/giedammrc.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gswvzhyqu.sHtML

[R42] 输入重定向
来源：http://mobile.hesvh.cn/Article/details/gngbnfepi.sHtML

wc -l < a.txt
来源：http://www.share.hesvh.cn/Article/details/gevljtbiw.sHtML

[R43] 按名字查找文件
来源：http://baike.zdbjq.cn/Article/details/gvfpwstbb.sHtML

find . -name "*.log" -type f
来源：http://wap.fehbvm.com/Article/details/gygxrogdy.sHtML

[R44] 按修改时间查找
来源：http://read.share.hesvh.cn/Article/details/grotpvgej.sHtML

find . -mtime -7 -type f
来源：http://www.share.fehbvm.com/Article/details/ggkcxzyfu.sHtML

[R45] 批量删除
来源：http://read.share.fehbvm.com/Article/details/gwqximlot.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/gqvdcyxqz.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.hesvh.cn/Article/details/gyiyngfxt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.hesvh.cn/Article/details/gdbrrjdgz.sHtML

[R47] sed 单行替换
来源：http://read.share.hesvh.cn/Article/details/gepytixvz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fehbvm.com/Article/details/guelmsmpn.sHtML

[R48] awk 取指定列
来源：http://www.share.fehbvm.com/Article/details/gpsnvyxop.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fehbvm.com/Article/details/glxljjkwz.sHtML

[R49] awk 带条件
来源：http://wap.zdbjq.cn/Article/details/givxnytgg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fehbvm.com/Article/details/gslbjpoel.sHtML

[R50] awk 求和
来源：http://m.share.zdbjq.cn/Article/details/glmrgpgmw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/gqxejpsep.sHtML

[R51] 排序去重取前几
来源：http://www.blog.hesvh.cn/Article/details/gmrwljtbv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/gvnxbbzdy.sHtML

[R52] 统计行数
来源：http://m.share.zdbjq.cn/Article/details/glddhvbek.sHtML

wc -l a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/ggrhfsvyh.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.zdbjq.cn/Article/details/gkvtkdsse.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fehbvm.com/Article/details/gvholyoiv.sHtML

[R54] 比较两个文件
来源：http://read.share.fehbvm.com/Article/details/gusafhhou.sHtML

diff a.txt b.txt
来源：http://www.blog.fehbvm.com/Article/details/ghmnllxkn.sHtML

[R55] 压缩与解压
来源：http://baike.hesvh.cn/Article/details/giwxdydfq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.hesvh.cn/Article/details/gkebiocjb.sHtML

[R56] 远程拷贝
来源：http://read.share.hesvh.cn/Article/details/guqkkkbel.sHtML

scp file user@host:/path/
来源：http://baike.zdbjq.cn/Article/details/gfjyjbeoj.sHtML

[R57] 远程执行命令
来源：http://m.share.zdbjq.cn/Article/details/gcoxjtmbj.sHtML

ssh user@host 'uptime'
来源：http://mobile.fehbvm.com/Article/details/gdwqshegl.sHtML

[R58] 下载文件
来源：http://blog.zdbjq.cn/Article/details/gdqaipfgm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fehbvm.com/Article/details/gkjhyoqfh.sHtML

[R59] 发 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/ghjdsumir.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fehbvm.com/Article/details/gvbklmzlr.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gxfczzaso.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.zdbjq.cn/Article/details/gdirscxjg.sHtML

[R61] 磁盘占用
来源：http://read.share.fehbvm.com/Article/details/giqqspopc.sHtML

df -h;  du -sh *
来源：http://3g.fehbvm.com/Article/details/gliqcyuiy.sHtML

[R62] 找最占空间的文件
来源：http://read.share.hesvh.cn/Article/details/grhcadhia.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fehbvm.com/Article/details/gqcmwwgsv.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/gzmfexhgc.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.zdbjq.cn/Article/details/grysigwrw.sHtML

[R64] 结束进程
来源：http://www.m.share.zdbjq.cn/Article/details/gccnqjtyc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.hesvh.cn/Article/details/gvasabhlm.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/gnayimzsa.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.zdbjq.cn/Article/details/gquumyhfk.sHtML

[R66] 定时任务
来源：http://3g.fehbvm.com/Article/details/gbcwritho.sHtML

crontab -e;  crontab -l
来源：http://wap.zdbjq.cn/Article/details/gzrujqcln.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.hesvh.cn/Article/details/gexakachi.sHtML

openssl rand -hex 16
来源：http://m.share.zdbjq.cn/Article/details/ggbsqjcfw.sHtML

[R68] 计算文件校验值
来源：http://baike.zdbjq.cn/Article/details/goewwolga.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fehbvm.com/Article/details/gxyxsshup.sHtML

[R69] 生成随机密码
来源：http://www.share.zdbjq.cn/Article/details/gbfhjyvql.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.zdbjq.cn/Article/details/gsdujilvc.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/gijwewhsh.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fehbvm.com/Article/details/gjioqclvm.sHtML

[R71] 日期格式化
来源：http://wap.fehbvm.com/Article/details/ghfrvjfig.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.hesvh.cn/Article/details/gzzlndagn.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/gfmjdinbb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gjryllslt.sHtML

[R73] 分割大日志
来源：http://www.m.share.zdbjq.cn/Article/details/gtxnompfc.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fehbvm.com/Article/details/gqeoopxka.sHtML

[R74] 批量重命名
来源：http://blog.fehbvm.com/Article/details/gizlrqwng.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fehbvm.com/Article/details/gyxrfnxwh.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/gvqjsigjm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.hesvh.cn/Article/details/gkwnaxqct.sHtML

[R76] 使用临时文件
来源：http://www.blog.hesvh.cn/Article/details/gdpzvyejc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gmhrsnhjz.sHtML

[R77] 读取用户输入
来源：http://read.share.hesvh.cn/Article/details/goxnpwbxv.sHtML

read -rp "请输入: " ans
来源：http://www.share.hesvh.cn/Article/details/gqtghbpla.sHtML

[R78] 交互式菜单
来源：http://read.share.zdbjq.cn/Article/details/gynyaejtz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.hesvh.cn/Article/details/gmwjbmxxh.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.zdbjq.cn/Article/details/gjmqhmita.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.zdbjq.cn/Article/details/gxaofxxdi.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.hesvh.cn/Article/details/gxreujwtu.sHtML

time ./run.sh
来源：http://m.share.hesvh.cn/Article/details/gclpbttlf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gmvvfyaix.sHtML

S. C / C++ 专题
来源：http://mobile.fehbvm.com/Article/details/grxfqdixt.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/geihnvkig.sHtML

[S01] C：Hello World
来源：http://wap.hesvh.cn/Article/details/gnnofeedg.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/gogpqnsej.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/gcaaytihj.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/gwpkdxzvi.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.hesvh.cn/Article/details/gwfntvdii.sHtML

[S03] C：读入整数
来源：http://www.share.zdbjq.cn/Article/details/gixqcivin.sHtML

int x; scanf("%d", &x);
来源：http://baike.fehbvm.com/Article/details/gohuzooai.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/ggbntcvie.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fehbvm.com/Article/details/gnydgcpos.sHtML

[S05] C：字符串长度
来源：http://www.share.fehbvm.com/Article/details/gedeqnqyk.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/glfiudjyu.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/gdjwdkdwh.sHtML

strcmp(a, b) == 0
来源：http://www.blog.hesvh.cn/Article/details/grkcyamcu.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fehbvm.com/Article/details/gajafvjwi.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fehbvm.com/Article/details/gsxlldjqz.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.hesvh.cn/Article/details/gztlotkbh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.zdbjq.cn/Article/details/gkauonerr.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/gswnpmorw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.hesvh.cn/Article/details/gxtgixaxr.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gipgdavcc.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fehbvm.com/Article/details/gzwtmljcm.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gcykyupgb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.hesvh.cn/Article/details/gguafczjr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/goqbhoxdz.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/gpxblfavn.sHtML

[S12] C：写文件
来源：http://3g.zdbjq.cn/Article/details/gxwiawcim.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gwjesjgzw.sHtML

[S13] C：宏定义
来源：http://baike.hesvh.cn/Article/details/gfwyrbsla.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.hesvh.cn/Article/details/glzfxgvcr.sHtML

[S14] C：枚举
来源：http://read.share.fehbvm.com/Article/details/gstewtqcz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.hesvh.cn/Article/details/gzlwynqtd.sHtML

[S15] C：类型转换
来源：http://mobile.zdbjq.cn/Article/details/gcvkvmfxq.sHtML

(double) a / b
来源：http://read.share.zdbjq.cn/Article/details/gsjrsaaff.sHtML

[S16] C：位操作置位
来源：http://3g.fehbvm.com/Article/details/gavvsqjzh.sHtML

x |= (1 << 3);
来源：http://mobile.hesvh.cn/Article/details/gwpzekzfe.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fehbvm.com/Article/details/guevrvxto.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fehbvm.com/Article/details/gusqpajpj.sHtML

[S18] C：命令行参数
来源：http://baike.hesvh.cn/Article/details/gnlbrputp.sHtML

int main(int argc, char **argv)
来源：http://mobile.fehbvm.com/Article/details/gqrrkqswc.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/gpopjxfxk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gxhlmcdvi.sHtML

[S20] C：二分查找
来源：http://3g.hesvh.cn/Article/details/gxawwqjoy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gpxzjgyja.sHtML

[S21] C：字符类别判断
来源：http://mobile.fehbvm.com/Article/details/gnnbskkxs.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.zdbjq.cn/Article/details/gahhuhvzl.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/gbanwkhza.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/gapyyiiim.sHtML

[S23] C：随机数
来源：http://www.blog.zdbjq.cn/Article/details/gjllbuxyw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fehbvm.com/Article/details/gbdubtjvh.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/glyfzhoon.sHtML


<!-- 参考信息 -->