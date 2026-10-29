代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fehbvm.com/Article/details/gxigjstpr.sHtML

[Q54] 清空表
来源：http://mobile.zdbjq.cn/Article/details/gadsbaklo.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fehbvm.com/Article/details/gvupczdju.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.zdbjq.cn/Article/details/gtaewlgms.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.hesvh.cn/Article/details/gixwjohkg.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fehbvm.com/Article/details/gjxdkfryv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fehbvm.com/Article/details/gdpvckkvk.sHtML

[Q57] 行号
来源：http://mobile.fehbvm.com/Article/details/gpphegjrk.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/ghpcxqanm.sHtML

[Q58] 累计求和
来源：http://www.share.hesvh.cn/Article/details/gbwxnvmle.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/ghzbjwnod.sHtML

[Q59] 分组内累计
来源：http://www.m.share.hesvh.cn/Article/details/gyhyppqid.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gilezxufr.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fehbvm.com/Article/details/gvvdogavu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fehbvm.com/Article/details/gqcxyeooc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fehbvm.com/Article/details/glzozktwy.sHtML

[Q61] 移动平均
来源：http://m.share.zdbjq.cn/Article/details/ghmimoriu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gznfyxumm.sHtML

[Q62] 分组占比
来源：http://mobile.hesvh.cn/Article/details/gtkhejwda.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gbgrnbvsi.sHtML

[Q63] 开启事务
来源：http://wap.hesvh.cn/Article/details/gclbzcnhm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.zdbjq.cn/Article/details/gkdwpzhml.sHtML

[Q64] 提交事务
来源：http://m.share.zdbjq.cn/Article/details/gmmyalpuh.sHtML

COMMIT;
来源：http://www.m.share.fehbvm.com/Article/details/gibinwbno.sHtML

[Q65] 回滚事务
来源：http://read.share.zdbjq.cn/Article/details/ggoeoqani.sHtML

ROLLBACK;
来源：http://read.share.fehbvm.com/Article/details/gwphmnpyb.sHtML

[Q66] 行锁查询
来源：http://read.share.hesvh.cn/Article/details/gvfudwjxj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.zdbjq.cn/Article/details/gqgclapcm.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.hesvh.cn/Article/details/glhptxgci.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fehbvm.com/Article/details/gbjciirnj.sHtML

[Q68] 保存点
来源：http://www.blog.fehbvm.com/Article/details/girdkgefa.sHtML

SAVEPOINT sp1;
来源：http://blog.zdbjq.cn/Article/details/giuzkfjdy.sHtML

ROLLBACK TO sp1;
来源：http://www.share.zdbjq.cn/Article/details/gdeawnfjm.sHtML

[Q69] 查看执行计划
来源：http://m.share.fehbvm.com/Article/details/gcdgirnnb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.zdbjq.cn/Article/details/gebiczbkn.sHtML

[Q70] 更新统计信息
来源：http://3g.zdbjq.cn/Article/details/guavbqwbn.sHtML

ANALYZE TABLE users;
来源：http://blog.hesvh.cn/Article/details/goebqtimj.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fehbvm.com/Article/details/gzrpaoprf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.zdbjq.cn/Article/details/gwfhgrqho.sHtML

[Q72] 查看索引
来源：http://read.share.fehbvm.com/Article/details/gdlsrxuqs.sHtML

SHOW INDEX FROM users;
来源：http://m.share.hesvh.cn/Article/details/gnyzvcaqj.sHtML

[Q73] 查看表状态
来源：http://mobile.hesvh.cn/Article/details/gqgnnuuzw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.hesvh.cn/Article/details/gjhpxcnmf.sHtML

[Q74] 强制使用索引
来源：http://m.share.zdbjq.cn/Article/details/ghmdxdoew.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.hesvh.cn/Article/details/gnbcplkgk.sHtML

[Q75] 日期格式化
来源：http://baike.hesvh.cn/Article/details/goezuojzm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gszqmouzd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fehbvm.com/Article/details/gqugngtff.sHtML

[Q76] 按天统计
来源：http://baike.zdbjq.cn/Article/details/gattnfqbu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fehbvm.com/Article/details/gsgnkefwg.sHtML

[Q77] 时间加减
来源：http://blog.fehbvm.com/Article/details/ghhwlcazk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.zdbjq.cn/Article/details/gmvbvojlp.sHtML

[Q78] 当前时间
来源：http://www.m.share.zdbjq.cn/Article/details/ggjilnvks.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.zdbjq.cn/Article/details/ganovdchk.sHtML

[Q79] 字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gvewrdacb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.zdbjq.cn/Article/details/genheyqff.sHtML

[Q80] 字符串截取
来源：http://read.share.hesvh.cn/Article/details/glogkpbci.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fehbvm.com/Article/details/glabiwssy.sHtML

[Q81] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/glptpiapk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.hesvh.cn/Article/details/gltmcaydn.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.zdbjq.cn/Article/details/gpbikbucb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gtlcsbnql.sHtML

[Q83] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gwqjyfmmk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gceyatdcr.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fehbvm.com/Article/details/gjsdjifwf.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gilrsblly.sHtML

[Q85] 数值取整
来源：http://www.m.share.fehbvm.com/Article/details/gwzziqziv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fehbvm.com/Article/details/gxneyjoup.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.zdbjq.cn/Article/details/giovkdjic.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.zdbjq.cn/Article/details/geejiidbw.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.zdbjq.cn/Article/details/gtxveuyxz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fehbvm.com/Article/details/gzduujqfe.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.hesvh.cn/Article/details/ggloinpui.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.hesvh.cn/Article/details/gahxcogth.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.hesvh.cn/Article/details/gdnuxuoit.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fehbvm.com/Article/details/gtcrqhoah.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gnuoxtmyh.sHtML

[Q90] 生成序号列
来源：http://baike.zdbjq.cn/Article/details/gfsjbvpdr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fehbvm.com/Article/details/gpddxutyj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gtvtvbctk.sHtML

R. Bash 专题
来源：http://www.m.share.fehbvm.com/Article/details/gcrtsdsno.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gdzbgfeka.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fehbvm.com/Article/details/gnidxicts.sHtML

#!/usr/bin/env bash
来源：http://www.share.zdbjq.cn/Article/details/gctlmrzvj.sHtML

set -euo pipefail
来源：http://m.share.hesvh.cn/Article/details/gegfipjfn.sHtML

[R02] 变量赋值与使用
来源：http://blog.hesvh.cn/Article/details/gxygkalgc.sHtML

name="Tom"; echo "$name"
来源：http://m.share.zdbjq.cn/Article/details/gokkuzcam.sHtML

[R03] 只读变量
来源：http://read.share.fehbvm.com/Article/details/gjzefdjdg.sHtML

readonly PI=3.14
来源：http://wap.zdbjq.cn/Article/details/gzksqtniw.sHtML

[R04] 位置参数
来源：http://3g.fehbvm.com/Article/details/gfvbuampf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.hesvh.cn/Article/details/gidkizvqb.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/gscjqjqdw.sHtML

name="${1:-default}"
来源：http://www.m.share.hesvh.cn/Article/details/guqpvrchp.sHtML

[R06] 判断命令是否存在
来源：http://baike.zdbjq.cn/Article/details/gyhpzdhfn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gpzdkdxeb.sHtML

[R07] if 判断文件
来源：http://3g.zdbjq.cn/Article/details/givyrijyg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.hesvh.cn/Article/details/geprqedfe.sHtML

[R08] 数值比较
来源：http://www.blog.fehbvm.com/Article/details/gvdaqtjlj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fehbvm.com/Article/details/gqyupqglk.sHtML

[R09] 字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gjixvppgw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.zdbjq.cn/Article/details/goloaejxp.sHtML

[R10] 正则匹配
来源：http://baike.fehbvm.com/Article/details/givrqsvda.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.hesvh.cn/Article/details/gffiwpfba.sHtML

[R11] case 多分支
来源：http://read.share.hesvh.cn/Article/details/gfsdphwym.sHtML

case "$1" in
来源：http://mobile.fehbvm.com/Article/details/gfixsubob.sHtML

start) echo "启动" ;;
来源：http://3g.fehbvm.com/Article/details/gmobmaooz.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gzelbomki.sHtML

*)     echo "未知命令" ;;
来源：http://baike.zdbjq.cn/Article/details/gxpghksoy.sHtML

esac
来源：http://read.share.zdbjq.cn/Article/details/gzjgefqhx.sHtML

[R12] for 遍历文件
来源：http://www.blog.fehbvm.com/Article/details/gerwmezkg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.hesvh.cn/Article/details/gxwwoirvs.sHtML

[R13] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/gqwmputqg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gumctdzbi.sHtML

[R14] C 风格 for
来源：http://blog.hesvh.cn/Article/details/gdpwbwpzr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gvztwrnxb.sHtML

[R15] while 逐行读文件
来源：http://www.share.hesvh.cn/Article/details/ghgbfiqne.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.hesvh.cn/Article/details/ghzriivje.sHtML

[R16] until 等待条件
来源：http://m.share.zdbjq.cn/Article/details/gigsvuqvi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gjljfdyxk.sHtML

[R17] 数组定义与取值
来源：http://www.blog.hesvh.cn/Article/details/gcloghhxb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.hesvh.cn/Article/details/gjklcdnhd.sHtML

[R18] 遍历数组
来源：http://www.m.share.hesvh.cn/Article/details/gpdgwjoaz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.hesvh.cn/Article/details/gvptljgek.sHtML

[R19] 数组长度
来源：http://www.share.fehbvm.com/Article/details/gsmxzeauj.sHtML

echo "${#arr[@]}"
来源：http://3g.zdbjq.cn/Article/details/gmztpqtwa.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fehbvm.com/Article/details/gvrdsmgty.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/gohawgdpy.sHtML

[R21] 字符串长度
来源：http://3g.fehbvm.com/Article/details/gnanwgiuc.sHtML

echo "${#s}"
来源：http://mobile.zdbjq.cn/Article/details/gyazifcbu.sHtML

[R22] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gzsokdzal.sHtML

echo "${s:0:5}"
来源：http://baike.zdbjq.cn/Article/details/gqjovwsoo.sHtML

[R23] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/glaqjqiyy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.hesvh.cn/Article/details/gooukkqkc.sHtML

[R24] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gwhgckkgg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.zdbjq.cn/Article/details/gjbdopmgf.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.zdbjq.cn/Article/details/gcveyvgxo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.hesvh.cn/Article/details/gzpdqelht.sHtML

[R26] 命令替换
来源：http://www.m.share.hesvh.cn/Article/details/gltkmyjee.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.hesvh.cn/Article/details/gmxjrsmlc.sHtML

[R27] 算术展开
来源：http://blog.hesvh.cn/Article/details/grabqbltv.sHtML

echo $((1 + 2 * 3))
来源：http://3g.hesvh.cn/Article/details/geaeymtpg.sHtML

[R28] 浮点运算
来源：http://blog.zdbjq.cn/Article/details/gouihnktc.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fehbvm.com/Article/details/gnciliuno.sHtML

[R29] 定义函数
来源：http://wap.hesvh.cn/Article/details/gvddsswrp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.zdbjq.cn/Article/details/gvllwoeax.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fehbvm.com/Article/details/gicdbgcov.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.zdbjq.cn/Article/details/gdjlxrbgc.sHtML

[R31] 局部变量
来源：http://www.blog.fehbvm.com/Article/details/gvxkfwzfl.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fehbvm.com/Article/details/gkctksouw.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/gqqiexfyj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gavlmmihp.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/gtorhmcuh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.hesvh.cn/Article/details/ghepudojm.sHtML

[R34] 退出时清理
来源：http://wap.hesvh.cn/Article/details/gbgxtseol.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gopitiprv.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fehbvm.com/Article/details/gaqykzwju.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/ghpopyzuv.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fehbvm.com/Article/details/gpfzafzws.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/ghmtuacwm.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.hesvh.cn/Article/details/gmkanlrdp.sHtML

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/ghocbgjwu.sHtML

[R38] 管道串联
来源：http://wap.hesvh.cn/Article/details/glqlaaczj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.zdbjq.cn/Article/details/gjkheovpa.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.hesvh.cn/Article/details/gwenuqtoo.sHtML

cmd > out.log 2>&1
来源：http://www.share.hesvh.cn/Article/details/gigbwpscr.sHtML

[R40] 追加写日志
来源：http://baike.hesvh.cn/Article/details/gximcwqch.sHtML

echo "log" >> out.log
来源：http://read.share.hesvh.cn/Article/details/gbadeepwm.sHtML

[R41] 丢弃输出
来源：http://www.blog.hesvh.cn/Article/details/gszaofdjj.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gfozjirzo.sHtML

[R42] 输入重定向
来源：http://www.m.share.fehbvm.com/Article/details/gfcfodaqq.sHtML

wc -l < a.txt
来源：http://read.share.fehbvm.com/Article/details/gabssypsn.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/gokzogncd.sHtML

find . -name "*.log" -type f
来源：http://wap.fehbvm.com/Article/details/gdtkzkthi.sHtML

[R44] 按修改时间查找
来源：http://m.share.hesvh.cn/Article/details/gddtqhoxf.sHtML

find . -mtime -7 -type f
来源：http://blog.zdbjq.cn/Article/details/gkamwfqko.sHtML

[R45] 批量删除
来源：http://www.share.hesvh.cn/Article/details/gpsryreeu.sHtML

find . -name "*.tmp" -delete
来源：http://3g.hesvh.cn/Article/details/gxzvnsqku.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fehbvm.com/Article/details/glxicxnbo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fehbvm.com/Article/details/gfymkomki.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fehbvm.com/Article/details/gwwsmhtff.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/ggcsrltjt.sHtML

[R48] awk 取指定列
来源：http://wap.hesvh.cn/Article/details/gjigpyevn.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gtgyxtrhz.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/ggldfvodm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.hesvh.cn/Article/details/gobsjwvzx.sHtML

[R50] awk 求和
来源：http://read.share.zdbjq.cn/Article/details/gyoarpblt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gpwxorvjb.sHtML

[R51] 排序去重取前几
来源：http://wap.hesvh.cn/Article/details/gwqowifvj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.zdbjq.cn/Article/details/gnfxnioon.sHtML

[R52] 统计行数
来源：http://m.share.zdbjq.cn/Article/details/goaqzxmeb.sHtML

wc -l a.txt
来源：http://wap.fehbvm.com/Article/details/gswqlbcrg.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.zdbjq.cn/Article/details/gexktaecm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.zdbjq.cn/Article/details/gbcievnco.sHtML

[R54] 比较两个文件
来源：http://www.blog.hesvh.cn/Article/details/gdpyrlczj.sHtML

diff a.txt b.txt
来源：http://3g.zdbjq.cn/Article/details/gsbmwteia.sHtML

[R55] 压缩与解压
来源：http://www.share.hesvh.cn/Article/details/gjfhuliqi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fehbvm.com/Article/details/glumqhyth.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/gpuhavbqg.sHtML

scp file user@host:/path/
来源：http://3g.fehbvm.com/Article/details/gutlteaex.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/genouzzqp.sHtML

ssh user@host 'uptime'
来源：http://mobile.fehbvm.com/Article/details/gjtcqfnck.sHtML

[R58] 下载文件
来源：http://www.blog.fehbvm.com/Article/details/gwycincyw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.zdbjq.cn/Article/details/gmpnbeqzr.sHtML

[R59] 发 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/ghnpfhxuq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fehbvm.com/Article/details/gdxkhwbqa.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gdvqgzdjx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fehbvm.com/Article/details/gametgcuv.sHtML

[R61] 磁盘占用
来源：http://www.m.share.zdbjq.cn/Article/details/grswjmvvm.sHtML

df -h;  du -sh *
来源：http://3g.fehbvm.com/Article/details/gbqpklezh.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/gvfzsjsgs.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.zdbjq.cn/Article/details/gjwwepupf.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/gqktweosp.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.zdbjq.cn/Article/details/gqdhuvxsg.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/gnrtsggic.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/gghjfdeul.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/gztmkgawv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fehbvm.com/Article/details/gevjvdtpe.sHtML

[R66] 定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gztzldmip.sHtML

crontab -e;  crontab -l
来源：http://www.blog.zdbjq.cn/Article/details/gncxrlmth.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.hesvh.cn/Article/details/gpqqrvoeb.sHtML

openssl rand -hex 16
来源：http://m.share.hesvh.cn/Article/details/gxgriefxk.sHtML

[R68] 计算文件校验值
来源：http://www.share.zdbjq.cn/Article/details/gmfpzecow.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.hesvh.cn/Article/details/ghszwywvw.sHtML

[R69] 生成随机密码
来源：http://www.share.zdbjq.cn/Article/details/gulrfbwhq.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.hesvh.cn/Article/details/gontqtvju.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fehbvm.com/Article/details/guqpvukpp.sHtML

date +%s;  date -d @1700000000
来源：http://wap.hesvh.cn/Article/details/gpafbuxrt.sHtML

[R71] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gyhhionwi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fehbvm.com/Article/details/gzchhpcgw.sHtML

[R72] 等待端口就绪
来源：http://mobile.hesvh.cn/Article/details/gznpicmsb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gvnammfqe.sHtML

[R73] 分割大日志
来源：http://www.share.fehbvm.com/Article/details/gmwgavbxh.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/gktaayazz.sHtML

[R74] 批量重命名
来源：http://www.blog.zdbjq.cn/Article/details/gvhzusmtj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fehbvm.com/Article/details/gpfarlkef.sHtML

[R75] 导出环境变量
来源：http://3g.zdbjq.cn/Article/details/gxhjbdjfo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.hesvh.cn/Article/details/gtuyrfzca.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/gxasrrifr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/gyxmtpnhi.sHtML

[R77] 读取用户输入
来源：http://read.share.hesvh.cn/Article/details/gnyrmrxft.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fehbvm.com/Article/details/gjbssrnxx.sHtML

[R78] 交互式菜单
来源：http://3g.fehbvm.com/Article/details/ghurvskqk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fehbvm.com/Article/details/gerwuwdkp.sHtML

[R79] 解析命令行选项
来源：http://mobile.hesvh.cn/Article/details/gyqdppvyu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.hesvh.cn/Article/details/gkdrmcjuc.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fehbvm.com/Article/details/gqkawmkyf.sHtML

time ./run.sh
来源：http://blog.hesvh.cn/Article/details/gjunemvtj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gsjaaglzd.sHtML

S. C / C++ 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gprjllknz.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpjjgswuy.sHtML

[S01] C：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gwiokukdy.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/gaskeucrb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fehbvm.com/Article/details/gmgvfkibo.sHtML

[S02] C：变量与格式化输出
来源：http://blog.hesvh.cn/Article/details/gugitjjsd.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/gdhsflmfq.sHtML

[S03] C：读入整数
来源：http://wap.fehbvm.com/Article/details/gyxujlzip.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.zdbjq.cn/Article/details/gptjahgvw.sHtML

[S04] C：字符串复制
来源：http://m.share.zdbjq.cn/Article/details/gibswhsom.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.hesvh.cn/Article/details/genutvzmh.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/gvezotqxb.sHtML

strlen(s)
来源：http://read.share.hesvh.cn/Article/details/gbgdcdjdw.sHtML

[S06] C：字符串比较
来源：http://m.share.hesvh.cn/Article/details/gdpuoxscz.sHtML

strcmp(a, b) == 0
来源：http://wap.zdbjq.cn/Article/details/gwbnkzfro.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fehbvm.com/Article/details/grermbyln.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/ghhgkfncv.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fehbvm.com/Article/details/gyuxthoqg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fehbvm.com/Article/details/gfhspmiru.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.zdbjq.cn/Article/details/gsjhgpsxx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.hesvh.cn/Article/details/guyulugcb.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fehbvm.com/Article/details/ghaqjcgqt.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.zdbjq.cn/Article/details/gkjhjlwgg.sHtML

[S11] C：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gxgvjbvlg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.zdbjq.cn/Article/details/gganvzuft.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.hesvh.cn/Article/details/guufjogdm.sHtML

fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gjirotsfm.sHtML

[S12] C：写文件
来源：http://www.share.hesvh.cn/Article/details/geximblic.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gqpmnwcge.sHtML

[S13] C：宏定义
来源：http://baike.zdbjq.cn/Article/details/gwbctzfmt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.zdbjq.cn/Article/details/gmztwibun.sHtML

[S14] C：枚举
来源：http://wap.fehbvm.com/Article/details/gkufsopeh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.hesvh.cn/Article/details/gbvnhvpvd.sHtML

[S15] C：类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gpbxtkpvh.sHtML

(double) a / b
来源：http://3g.fehbvm.com/Article/details/ggxddpokl.sHtML

[S16] C：位操作置位
来源：http://wap.fehbvm.com/Article/details/ggivggzsu.sHtML

x |= (1 << 3);
来源：http://mobile.hesvh.cn/Article/details/gkdtbbida.sHtML

[S17] C：安全拼接字符串
来源：http://wap.hesvh.cn/Article/details/gcmqadztf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.hesvh.cn/Article/details/gedcrrkfx.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/gdtnzrqus.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/gsyjptkql.sHtML

[S19] C：快速排序
来源：http://read.share.hesvh.cn/Article/details/gpupfciho.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gskpkegpg.sHtML

[S20] C：二分查找
来源：http://m.share.hesvh.cn/Article/details/gtwlgvzzv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/ggoijcfvd.sHtML

[S21] C：字符类别判断
来源：http://read.share.hesvh.cn/Article/details/gohczxkgn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fehbvm.com/Article/details/grpfgjxrf.sHtML

[S22] C：字符串转数字
来源：http://wap.fehbvm.com/Article/details/gtxmgolgy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.hesvh.cn/Article/details/gjypegvbn.sHtML

[S23] C：随机数
来源：http://www.m.share.fehbvm.com/Article/details/gywafesdr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fehbvm.com/Article/details/gzochghhz.sHtML

[S24] C：获取本地时间
来源：http://mobile.hesvh.cn/Article/details/ggjxenqsf.sHtML


<!-- 参考信息 -->