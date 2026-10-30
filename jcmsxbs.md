代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.hesvh.cn/Article/details/gkzwryell.sHtML

[Q52] 删除指定行
来源：http://blog.fehbvm.com/Article/details/gswbfkvdz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gmyjyocfn.sHtML

[Q53] 按条件删除
来源：http://blog.zdbjq.cn/Article/details/gngsvojxk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.hesvh.cn/Article/details/glhnaqcfa.sHtML

[Q54] 清空表
来源：http://baike.hesvh.cn/Article/details/ggdzzcmzt.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fehbvm.com/Article/details/gowakutbd.sHtML

[Q55] 排名（并列占位）
来源：http://3g.zdbjq.cn/Article/details/gjbvlwxdz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gpnmyeogb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.zdbjq.cn/Article/details/gikqjkiem.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.hesvh.cn/Article/details/gxbgtlfoy.sHtML

[Q57] 行号
来源：http://read.share.hesvh.cn/Article/details/gylmilbze.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.zdbjq.cn/Article/details/ghdqhuskd.sHtML

[Q58] 累计求和
来源：http://3g.zdbjq.cn/Article/details/gtukssorv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gmrmjqgjz.sHtML

[Q59] 分组内累计
来源：http://www.blog.hesvh.cn/Article/details/gibngkskw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gonnixbaz.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gtjcqltyf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.zdbjq.cn/Article/details/gpbdryaac.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gfdzpppkq.sHtML

[Q61] 移动平均
来源：http://wap.hesvh.cn/Article/details/gqlrtshsx.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gmnyadclc.sHtML

[Q62] 分组占比
来源：http://wap.hesvh.cn/Article/details/gmtgrfkzi.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gsbhrrdpa.sHtML

[Q63] 开启事务
来源：http://read.share.hesvh.cn/Article/details/gundtlwbd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.zdbjq.cn/Article/details/gbxvkngwn.sHtML

[Q64] 提交事务
来源：http://baike.fehbvm.com/Article/details/gfoijughq.sHtML

COMMIT;
来源：http://mobile.fehbvm.com/Article/details/gxnjoxsoa.sHtML

[Q65] 回滚事务
来源：http://blog.zdbjq.cn/Article/details/gyhzyiqhh.sHtML

ROLLBACK;
来源：http://www.blog.fehbvm.com/Article/details/gnxtinyaq.sHtML

[Q66] 行锁查询
来源：http://3g.fehbvm.com/Article/details/gpqkzgtcx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fehbvm.com/Article/details/gunhsuaxk.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.hesvh.cn/Article/details/gaopbaagt.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.zdbjq.cn/Article/details/gphxnrjdh.sHtML

[Q68] 保存点
来源：http://www.m.share.zdbjq.cn/Article/details/gaeyhhhrs.sHtML

SAVEPOINT sp1;
来源：http://wap.fehbvm.com/Article/details/gzmnjrvel.sHtML

ROLLBACK TO sp1;
来源：http://blog.zdbjq.cn/Article/details/gzhwszgnm.sHtML

[Q69] 查看执行计划
来源：http://m.share.zdbjq.cn/Article/details/gbjlvtpwt.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.hesvh.cn/Article/details/gcsmoulsl.sHtML

[Q70] 更新统计信息
来源：http://blog.zdbjq.cn/Article/details/gjxdiscbw.sHtML

ANALYZE TABLE users;
来源：http://blog.zdbjq.cn/Article/details/gkmrrqgtw.sHtML

[Q71] 查看建表语句
来源：http://mobile.hesvh.cn/Article/details/gmhiubyro.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fehbvm.com/Article/details/grbabmiap.sHtML

[Q72] 查看索引
来源：http://www.blog.hesvh.cn/Article/details/gnsmoemnd.sHtML

SHOW INDEX FROM users;
来源：http://m.share.hesvh.cn/Article/details/gicpqfvua.sHtML

[Q73] 查看表状态
来源：http://wap.fehbvm.com/Article/details/gsktkxauq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fehbvm.com/Article/details/gyogauacb.sHtML

[Q74] 强制使用索引
来源：http://3g.hesvh.cn/Article/details/gzaenddrt.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fehbvm.com/Article/details/ghezdwlhe.sHtML

[Q75] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/ghhznhqdl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.hesvh.cn/Article/details/ggeegpdor.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.zdbjq.cn/Article/details/gzuxyvepe.sHtML

[Q76] 按天统计
来源：http://mobile.fehbvm.com/Article/details/glodvymok.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fehbvm.com/Article/details/gylrjzdyj.sHtML

[Q77] 时间加减
来源：http://www.share.zdbjq.cn/Article/details/gsxhywuav.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.hesvh.cn/Article/details/ganztigha.sHtML

[Q78] 当前时间
来源：http://www.m.share.fehbvm.com/Article/details/gzqfkrwmx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.hesvh.cn/Article/details/gypfykwyz.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/guqmwkork.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.zdbjq.cn/Article/details/gjalxtlmo.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fehbvm.com/Article/details/gnsikbhnm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gpovzskxr.sHtML

[Q81] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gctdcgldc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.zdbjq.cn/Article/details/glpsiucsj.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.zdbjq.cn/Article/details/guubalqbp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/ghlxkqyko.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gxoykmpll.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gbzmvdmjy.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.zdbjq.cn/Article/details/gfhzsvqyw.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gttlxiwbl.sHtML

[Q85] 数值取整
来源：http://m.share.zdbjq.cn/Article/details/gxybnoyir.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.hesvh.cn/Article/details/gglmwniit.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.hesvh.cn/Article/details/gdumtnvzi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.hesvh.cn/Article/details/gmkwtjdoy.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/gvugvfgqj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.zdbjq.cn/Article/details/gqmegsatr.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.hesvh.cn/Article/details/grgahucmm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.hesvh.cn/Article/details/gllerdjxw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.hesvh.cn/Article/details/gjqzatsxf.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fehbvm.com/Article/details/gewgqkojb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gscmpkmks.sHtML

[Q90] 生成序号列
来源：http://www.blog.hesvh.cn/Article/details/glkyagsjk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.zdbjq.cn/Article/details/gzhjtxefa.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghirjwqnq.sHtML

R. Bash 专题
来源：http://read.share.fehbvm.com/Article/details/gveeqztgu.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gtfqxsfdn.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fehbvm.com/Article/details/gdblfanes.sHtML

#!/usr/bin/env bash
来源：http://blog.fehbvm.com/Article/details/gzyvkcois.sHtML

set -euo pipefail
来源：http://3g.fehbvm.com/Article/details/gzuquphxy.sHtML

[R02] 变量赋值与使用
来源：http://wap.zdbjq.cn/Article/details/gedsgtkbg.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fehbvm.com/Article/details/gcgppihuy.sHtML

[R03] 只读变量
来源：http://www.share.fehbvm.com/Article/details/gniojkvec.sHtML

readonly PI=3.14
来源：http://www.m.share.fehbvm.com/Article/details/gfqvhucgi.sHtML

[R04] 位置参数
来源：http://wap.hesvh.cn/Article/details/gbuchdxxz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.zdbjq.cn/Article/details/guhsmvxev.sHtML

[R05] 参数默认值
来源：http://wap.hesvh.cn/Article/details/gceogrqrb.sHtML

name="${1:-default}"
来源：http://www.share.hesvh.cn/Article/details/grvbwfbxa.sHtML

[R06] 判断命令是否存在
来源：http://baike.fehbvm.com/Article/details/glmeddxdj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gyckxxzlh.sHtML

[R07] if 判断文件
来源：http://read.share.zdbjq.cn/Article/details/gqubkozjf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fehbvm.com/Article/details/gatjmrzia.sHtML

[R08] 数值比较
来源：http://mobile.fehbvm.com/Article/details/gmlofwsfx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.hesvh.cn/Article/details/gqsevvfww.sHtML

[R09] 字符串比较
来源：http://mobile.fehbvm.com/Article/details/gokbgkniz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.hesvh.cn/Article/details/gkpqnidkf.sHtML

[R10] 正则匹配
来源：http://3g.hesvh.cn/Article/details/gjmancqia.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.hesvh.cn/Article/details/gpmjvyapj.sHtML

[R11] case 多分支
来源：http://blog.hesvh.cn/Article/details/grehhxycl.sHtML

case "$1" in
来源：http://3g.hesvh.cn/Article/details/ghrrchtpj.sHtML

start) echo "启动" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gsbkskzor.sHtML

stop)  echo "停止" ;;
来源：http://wap.hesvh.cn/Article/details/gmcjlhivd.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gttbtnpng.sHtML

esac
来源：http://www.m.share.fehbvm.com/Article/details/gapxibuwb.sHtML

[R12] for 遍历文件
来源：http://www.blog.zdbjq.cn/Article/details/gozlzduem.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fehbvm.com/Article/details/gaxhdxkam.sHtML

[R13] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/gecxzjixy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gpsgkkswi.sHtML

[R14] C 风格 for
来源：http://wap.zdbjq.cn/Article/details/ghntmwywu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gqscxgudk.sHtML

[R15] while 逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gvkjeflls.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.zdbjq.cn/Article/details/gggquitrb.sHtML

[R16] until 等待条件
来源：http://baike.hesvh.cn/Article/details/gbslpfuas.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gbwzgjfxm.sHtML

[R17] 数组定义与取值
来源：http://wap.fehbvm.com/Article/details/gxvocwhbg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.hesvh.cn/Article/details/gbdipzxmq.sHtML

[R18] 遍历数组
来源：http://baike.zdbjq.cn/Article/details/giulyypgi.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fehbvm.com/Article/details/ggkcgbwaw.sHtML

[R19] 数组长度
来源：http://baike.zdbjq.cn/Article/details/ghbdgpiez.sHtML

echo "${#arr[@]}"
来源：http://3g.zdbjq.cn/Article/details/gkdztclyg.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.zdbjq.cn/Article/details/gfzqdkvln.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.hesvh.cn/Article/details/gudbsgcpv.sHtML

[R21] 字符串长度
来源：http://3g.zdbjq.cn/Article/details/gyawmbwwf.sHtML

echo "${#s}"
来源：http://blog.hesvh.cn/Article/details/gbmtkobzx.sHtML

[R22] 截取子串
来源：http://www.share.fehbvm.com/Article/details/grcvguyza.sHtML

echo "${s:0:5}"
来源：http://www.share.fehbvm.com/Article/details/gsikbbeoy.sHtML

[R23] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gmtuipkeo.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.zdbjq.cn/Article/details/gzrnpkrnw.sHtML

[R24] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gqrxekqux.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fehbvm.com/Article/details/gsypwqomd.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.zdbjq.cn/Article/details/ghkkklegx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.hesvh.cn/Article/details/gouyzoqsu.sHtML

[R26] 命令替换
来源：http://read.share.hesvh.cn/Article/details/gseklsxuv.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.zdbjq.cn/Article/details/gcpzvnfzs.sHtML

[R27] 算术展开
来源：http://3g.hesvh.cn/Article/details/gkxphbjhn.sHtML

echo $((1 + 2 * 3))
来源：http://baike.zdbjq.cn/Article/details/gxfukcisx.sHtML

[R28] 浮点运算
来源：http://www.blog.hesvh.cn/Article/details/gdaqjlnmd.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.hesvh.cn/Article/details/goqwzpdvg.sHtML

[R29] 定义函数
来源：http://blog.hesvh.cn/Article/details/glulpykwf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.zdbjq.cn/Article/details/gsrozkcaq.sHtML

[R30] 函数返回状态码
来源：http://m.share.zdbjq.cn/Article/details/ghlqzybvj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.zdbjq.cn/Article/details/gmltwwytc.sHtML

[R31] 局部变量
来源：http://www.m.share.fehbvm.com/Article/details/glikkwujh.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fehbvm.com/Article/details/gwmhxerpd.sHtML

[R32] 参数个数校验
来源：http://m.share.hesvh.cn/Article/details/guxllzofx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gslohsbga.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fehbvm.com/Article/details/gtarvnpmo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.zdbjq.cn/Article/details/gsgyanxea.sHtML

[R34] 退出时清理
来源：http://m.share.fehbvm.com/Article/details/gthyvpgtp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/ghugdihyh.sHtML

[R35] 后台执行并等待
来源：http://baike.zdbjq.cn/Article/details/gzmhgtnhb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.hesvh.cn/Article/details/gkpedwiqm.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fehbvm.com/Article/details/gyherboqs.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/gfvousyax.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fehbvm.com/Article/details/gayqzdsjm.sHtML

files=$(ls -1)
来源：http://3g.zdbjq.cn/Article/details/gkoffyxis.sHtML

[R38] 管道串联
来源：http://read.share.hesvh.cn/Article/details/gtskveztf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.zdbjq.cn/Article/details/gwwdvvcpe.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fehbvm.com/Article/details/gcnwffanr.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gdupcvcjt.sHtML

[R40] 追加写日志
来源：http://www.blog.hesvh.cn/Article/details/ggxizbvtk.sHtML

echo "log" >> out.log
来源：http://www.share.zdbjq.cn/Article/details/getbygmaz.sHtML

[R41] 丢弃输出
来源：http://wap.zdbjq.cn/Article/details/gjbunytaw.sHtML

cmd >/dev/null 2>&1
来源：http://baike.hesvh.cn/Article/details/gcsnaxcay.sHtML

[R42] 输入重定向
来源：http://3g.hesvh.cn/Article/details/gbnmrvcbg.sHtML

wc -l < a.txt
来源：http://blog.zdbjq.cn/Article/details/goeeowjiw.sHtML

[R43] 按名字查找文件
来源：http://m.share.fehbvm.com/Article/details/gggpwvoeg.sHtML

find . -name "*.log" -type f
来源：http://baike.hesvh.cn/Article/details/grkhdtmsn.sHtML

[R44] 按修改时间查找
来源：http://mobile.fehbvm.com/Article/details/gpmzafuik.sHtML

find . -mtime -7 -type f
来源：http://baike.hesvh.cn/Article/details/guovscdsc.sHtML

[R45] 批量删除
来源：http://www.m.share.fehbvm.com/Article/details/gxajutkmh.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fehbvm.com/Article/details/gbeblhsyp.sHtML

[R46] 递归替换文件内容
来源：http://mobile.hesvh.cn/Article/details/gwqmhvunr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fehbvm.com/Article/details/gqoeszopd.sHtML

[R47] sed 单行替换
来源：http://m.share.zdbjq.cn/Article/details/gmnhujost.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.hesvh.cn/Article/details/gdsclmmwn.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/ggqkbpugh.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gkzzjlryt.sHtML

[R49] awk 带条件
来源：http://wap.fehbvm.com/Article/details/gyreaibtn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.hesvh.cn/Article/details/gkkkzpsae.sHtML

[R50] awk 求和
来源：http://mobile.fehbvm.com/Article/details/gdsflqngk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gpttkqzgj.sHtML

[R51] 排序去重取前几
来源：http://www.share.zdbjq.cn/Article/details/gdqdhjevk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.zdbjq.cn/Article/details/gbqjuycmg.sHtML

[R52] 统计行数
来源：http://www.m.share.hesvh.cn/Article/details/gnexnaghx.sHtML

wc -l a.txt
来源：http://3g.hesvh.cn/Article/details/gxkxwexbq.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.hesvh.cn/Article/details/gtkljyxzf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.zdbjq.cn/Article/details/gwongjpxd.sHtML

[R54] 比较两个文件
来源：http://wap.hesvh.cn/Article/details/gzyjuqcaw.sHtML

diff a.txt b.txt
来源：http://blog.hesvh.cn/Article/details/glzoulivq.sHtML

[R55] 压缩与解压
来源：http://www.share.zdbjq.cn/Article/details/gvoixawmj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fehbvm.com/Article/details/gltrvkkov.sHtML

[R56] 远程拷贝
来源：http://www.share.fehbvm.com/Article/details/gquolkvpb.sHtML

scp file user@host:/path/
来源：http://blog.fehbvm.com/Article/details/gbkzfmxpa.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/gbbigqlja.sHtML

ssh user@host 'uptime'
来源：http://m.share.zdbjq.cn/Article/details/gifetmpre.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/gvbxczgff.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fehbvm.com/Article/details/gqjpzasmc.sHtML

[R59] 发 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gqrwjfkub.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fehbvm.com/Article/details/gzjfddjea.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/guzjdpzdf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fehbvm.com/Article/details/gdbjnbhsp.sHtML

[R61] 磁盘占用
来源：http://read.share.hesvh.cn/Article/details/gguchlxcs.sHtML

df -h;  du -sh *
来源：http://3g.zdbjq.cn/Article/details/gckyrhozt.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fehbvm.com/Article/details/gvfbrdvlf.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.hesvh.cn/Article/details/gyynxerhz.sHtML

[R63] 内存与进程
来源：http://blog.hesvh.cn/Article/details/gdcbunwxf.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.hesvh.cn/Article/details/gyvksonrm.sHtML

[R64] 结束进程
来源：http://m.share.fehbvm.com/Article/details/gnfrbikmy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.zdbjq.cn/Article/details/ghjizfxit.sHtML

[R65] 查看端口占用
来源：http://m.share.fehbvm.com/Article/details/gwskkzeyq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.zdbjq.cn/Article/details/gvfnlayjg.sHtML

[R66] 定时任务
来源：http://read.share.fehbvm.com/Article/details/guugevlyb.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fehbvm.com/Article/details/gksvaiblj.sHtML

[R67] 生成随机十六进制串
来源：http://baike.zdbjq.cn/Article/details/gfprcpjab.sHtML

openssl rand -hex 16
来源：http://wap.zdbjq.cn/Article/details/gglwujrcn.sHtML

[R68] 计算文件校验值
来源：http://blog.fehbvm.com/Article/details/gejldzwdi.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.hesvh.cn/Article/details/gxbkuxmse.sHtML

[R69] 生成随机密码
来源：http://www.share.hesvh.cn/Article/details/gfaucxrfu.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.hesvh.cn/Article/details/gpkyyxzmc.sHtML

[R70] 时间戳与互转
来源：http://www.share.hesvh.cn/Article/details/gbwsboefx.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.zdbjq.cn/Article/details/gdfkeqpiy.sHtML

[R71] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gguncrfbg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.zdbjq.cn/Article/details/giknsquoj.sHtML

[R72] 等待端口就绪
来源：http://read.share.zdbjq.cn/Article/details/goymguhbn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gvsemwdph.sHtML

[R73] 分割大日志
来源：http://read.share.hesvh.cn/Article/details/gpjfzirft.sHtML

split -l 1000 big.log part_
来源：http://3g.hesvh.cn/Article/details/gfrvzzgjf.sHtML

[R74] 批量重命名
来源：http://www.share.zdbjq.cn/Article/details/gztoaujhy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fehbvm.com/Article/details/gutsityoy.sHtML

[R75] 导出环境变量
来源：http://m.share.fehbvm.com/Article/details/glhgohnih.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/gxdvpfofm.sHtML

[R76] 使用临时文件
来源：http://www.blog.fehbvm.com/Article/details/gpqfxyvrd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gvtsgobtf.sHtML

[R77] 读取用户输入
来源：http://3g.fehbvm.com/Article/details/gdcnsygoj.sHtML

read -rp "请输入: " ans
来源：http://www.share.hesvh.cn/Article/details/giimuqrme.sHtML

[R78] 交互式菜单
来源：http://m.share.hesvh.cn/Article/details/gshjwklkp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fehbvm.com/Article/details/gengcnuru.sHtML

[R79] 解析命令行选项
来源：http://3g.fehbvm.com/Article/details/gquezxhdj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.zdbjq.cn/Article/details/gxhczoqno.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.hesvh.cn/Article/details/grsonracl.sHtML

time ./run.sh
来源：http://blog.hesvh.cn/Article/details/gyfbisqhg.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gpbkzruir.sHtML

S. C / C++ 专题
来源：http://wap.fehbvm.com/Article/details/gugqrokcf.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmgwinoav.sHtML

[S01] C：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gmzssmsar.sHtML

#include <stdio.h>
来源：http://read.share.fehbvm.com/Article/details/grjeodxxq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.zdbjq.cn/Article/details/gmbusqjnz.sHtML

[S02] C：变量与格式化输出
来源：http://baike.hesvh.cn/Article/details/gdgyogbtg.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.zdbjq.cn/Article/details/gkfalitwq.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/giwonxmyh.sHtML

int x; scanf("%d", &x);
来源：http://baike.hesvh.cn/Article/details/gfeimqgqk.sHtML

[S04] C：字符串复制
来源：http://mobile.hesvh.cn/Article/details/gcwqbwaus.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.zdbjq.cn/Article/details/gdmqhlape.sHtML

[S05] C：字符串长度
来源：http://baike.fehbvm.com/Article/details/ghfzdsznq.sHtML

strlen(s)
来源：http://blog.zdbjq.cn/Article/details/gzfidvzga.sHtML

[S06] C：字符串比较
来源：http://blog.zdbjq.cn/Article/details/gptmgcspd.sHtML

strcmp(a, b) == 0
来源：http://read.share.zdbjq.cn/Article/details/ggejghtpa.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fehbvm.com/Article/details/gkfjlgsos.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.hesvh.cn/Article/details/gltazyymw.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.zdbjq.cn/Article/details/gginxkwku.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/gwazymzot.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.hesvh.cn/Article/details/gywadsaad.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.hesvh.cn/Article/details/ggxkngruk.sHtML

[S10] C：指针与解引用
来源：http://mobile.fehbvm.com/Article/details/gptlkgzne.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fehbvm.com/Article/details/gmpodsjlf.sHtML

[S11] C：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gtzgkrnpk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.hesvh.cn/Article/details/gynamhkxc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.hesvh.cn/Article/details/gnqslukkr.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/grpnzephd.sHtML

[S12] C：写文件
来源：http://read.share.fehbvm.com/Article/details/gelrihnwp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gxzdqdcdi.sHtML

[S13] C：宏定义
来源：http://www.share.hesvh.cn/Article/details/gdowxymdk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.hesvh.cn/Article/details/geivwvdxp.sHtML

[S14] C：枚举
来源：http://wap.zdbjq.cn/Article/details/gdpekmlyb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.zdbjq.cn/Article/details/gpeomctfz.sHtML

[S15] C：类型转换
来源：http://read.share.hesvh.cn/Article/details/ghomyljjn.sHtML

(double) a / b
来源：http://read.share.hesvh.cn/Article/details/gkjkqelej.sHtML

[S16] C：位操作置位
来源：http://wap.hesvh.cn/Article/details/gjnifkqqi.sHtML

x |= (1 << 3);
来源：http://www.share.zdbjq.cn/Article/details/gnejdomdd.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/gyckltist.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.zdbjq.cn/Article/details/gbtyvoqkd.sHtML

[S18] C：命令行参数
来源：http://m.share.hesvh.cn/Article/details/ghzdlwpnw.sHtML

int main(int argc, char **argv)
来源：http://blog.hesvh.cn/Article/details/gnkljgoev.sHtML

[S19] C：快速排序
来源：http://read.share.zdbjq.cn/Article/details/gnaakbbtz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gqixzkniz.sHtML

[S20] C：二分查找
来源：http://3g.fehbvm.com/Article/details/gdyajphll.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gajfufech.sHtML

[S21] C：字符类别判断
来源：http://www.blog.zdbjq.cn/Article/details/gmlbjfakp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.hesvh.cn/Article/details/gvxtvcxea.sHtML

[S22] C：字符串转数字
来源：http://m.share.fehbvm.com/Article/details/grqczdknh.sHtML


<!-- 参考信息 -->