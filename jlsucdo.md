代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggggjufqr.sHtML

[Q58] 累计求和
来源：http://baike.fanxiaobao.xyz/Article/details/gwgoqbgdg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlrmukxe.sHtML

[Q59] 分组内累计
来源：http://3g.fanxiaobao.xyz/Article/details/gnpprmhpp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewomnold.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fanxiaobao.xyz/Article/details/garhaxcke.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gughxhgjr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgmgatqc.sHtML

[Q61] 移动平均
来源：http://read.share.fanxiaobao.xyz/Article/details/gcyuwtwiv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gxowmjlwx.sHtML

[Q62] 分组占比
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmfqqhaw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gpirqdjyb.sHtML

[Q63] 开启事务
来源：http://3g.fanxiaobao.xyz/Article/details/goqirbemq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvglihgf.sHtML

[Q64] 提交事务
来源：http://3g.fanxiaobao.xyz/Article/details/gwbbtmryj.sHtML

COMMIT;
来源：http://read.share.fanxiaobao.xyz/Article/details/gglnhcnkf.sHtML

[Q65] 回滚事务
来源：http://3g.fanxiaobao.xyz/Article/details/gbdnzqjor.sHtML

ROLLBACK;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyakkfdeg.sHtML

[Q66] 行锁查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxqxcrmu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fanxiaobao.xyz/Article/details/gqqypvmeb.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fanxiaobao.xyz/Article/details/gvlpqhwem.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fanxiaobao.xyz/Article/details/guepggoda.sHtML

[Q68] 保存点
来源：http://baike.fanxiaobao.xyz/Article/details/ghklekpdw.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljqgczyb.sHtML

ROLLBACK TO sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gzksrploc.sHtML

[Q69] 查看执行计划
来源：http://blog.fanxiaobao.xyz/Article/details/greahqgsc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fanxiaobao.xyz/Article/details/gthsbdeyr.sHtML

[Q70] 更新统计信息
来源：http://blog.fanxiaobao.xyz/Article/details/gvcsxbpdk.sHtML

ANALYZE TABLE users;
来源：http://m.share.fanxiaobao.xyz/Article/details/guluomhst.sHtML

[Q71] 查看建表语句
来源：http://www.share.fanxiaobao.xyz/Article/details/gebcgovtz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fanxiaobao.xyz/Article/details/grozjosjq.sHtML

[Q72] 查看索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gowauzdgm.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggaiqbqca.sHtML

[Q73] 查看表状态
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfgqikvd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gabauhrzn.sHtML

[Q74] 强制使用索引
来源：http://3g.fanxiaobao.xyz/Article/details/gnzcuwcxu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fanxiaobao.xyz/Article/details/gyltcdqwa.sHtML

[Q75] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/geaenwuce.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gueeacekg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fanxiaobao.xyz/Article/details/gfpwpxbah.sHtML

[Q76] 按天统计
来源：http://baike.fanxiaobao.xyz/Article/details/ghlywhykb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgezxcdq.sHtML

[Q77] 时间加减
来源：http://baike.fanxiaobao.xyz/Article/details/ggmeihkpg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fanxiaobao.xyz/Article/details/giwslxxjp.sHtML

[Q78] 当前时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gtaffgrfm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fanxiaobao.xyz/Article/details/gnuxksedl.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprwlwccz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fanxiaobao.xyz/Article/details/gifbevzld.sHtML

[Q80] 字符串截取
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnvyxzan.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gecvubjtd.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/ggswaejre.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gcdocogto.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fanxiaobao.xyz/Article/details/gbimwlrdk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgnekqxp.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocmplisa.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozenrfqe.sHtML

[Q84] 去除首尾空格
来源：http://baike.fanxiaobao.xyz/Article/details/ghnudeiqw.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gxhnaljlq.sHtML

[Q85] 数值取整
来源：http://wap.fanxiaobao.xyz/Article/details/gqmeacdyl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fanxiaobao.xyz/Article/details/gcertunxb.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fanxiaobao.xyz/Article/details/gqojuglls.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/gqeasrxsw.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtsrjzugk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbdhrirm.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtpxmwdc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fanxiaobao.xyz/Article/details/gsbsdemez.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnndzyyzh.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/glgeqifit.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhalfbis.sHtML

[Q90] 生成序号列
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxojgrgo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fanxiaobao.xyz/Article/details/gddrydmrm.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/glpwjzkca.sHtML

R. Bash 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gtamlrvny.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgqozwdx.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaptvsyzf.sHtML

#!/usr/bin/env bash
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtbfrzym.sHtML

set -euo pipefail
来源：http://m.share.fanxiaobao.xyz/Article/details/gpitafzsz.sHtML

[R02] 变量赋值与使用
来源：http://3g.fanxiaobao.xyz/Article/details/glftzcyrz.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwldjbldr.sHtML

[R03] 只读变量
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmvyphss.sHtML

readonly PI=3.14
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjommvdx.sHtML

[R04] 位置参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgvcisps.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fanxiaobao.xyz/Article/details/gmdkldajx.sHtML

[R05] 参数默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gyrkwichw.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gzfocplbv.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gywzbxvnr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfqsrvig.sHtML

[R07] if 判断文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbsnszke.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gcziggloj.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxgjdhdo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsvzdkvq.sHtML

[R09] 字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gdcevxpno.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgdzhhho.sHtML

[R10] 正则匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/guibcssir.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gxzdunyjf.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/gpudqvwap.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfajdyvo.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/giulbfzus.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvsicnzpg.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gancmuxxw.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/gvuaupuzi.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrzfqfkb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokkyntrn.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/grggrilio.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gxouczoky.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/gywqegxma.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gadqvhxmd.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gwklgglmo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/godwqxjjw.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/gelnapmtv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqmvxasz.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/grnoabyqd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxixqrhd.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/gzagsxrcd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyagqckku.sHtML

[R19] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkanpvewi.sHtML

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgikrkii.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsurnmqpm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gbiimlurp.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gghshssoo.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsicaqra.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/gsedeetwy.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrfhvvdw.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/ggsgrjytq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfcabsmf.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gyngohjuw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtsshkec.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbtckzkp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbxnamqx.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gipvdqnyz.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkcxinof.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gqcojqvgd.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/giysrbpqy.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gyifzzaev.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkwvfkhn.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumuvaows.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxecqyrjk.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gwleqphih.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/ghiurulvv.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/guozqbobo.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fanxiaobao.xyz/Article/details/grsxaslkr.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/grahfntne.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzipfisd.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkzxunqf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzaxubjp.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjzmaxyt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gygvicjpp.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gmnqvyigv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrsgkbmh.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gezmwpxcg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/gtynwfwxu.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnumpwmtq.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvrsaclp.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/gqurqsltq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/gptoktdhb.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/gkqpjuamr.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gxausreqo.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvnbkqqb.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gecwhpogc.sHtML

[R41] 丢弃输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwwmafok.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/grcimaeac.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/gbeubgktv.sHtML

wc -l < a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcwkkhzq.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/gibodjbmg.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gsitafiyu.sHtML

[R44] 按修改时间查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gykpxrzja.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gtwtqgvyb.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/giwtzcexd.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkbgigba.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykpygzvw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gxlxumuji.sHtML

[R47] sed 单行替换
来源：http://baike.fanxiaobao.xyz/Article/details/gqjutygzq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gtxlzanbb.sHtML

[R48] awk 取指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdepovoy.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfwrgoys.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/gsuvhfkpi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlujdunk.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gslpfpeei.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gzgxbtdcr.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geflkbeho.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/gxogcrsze.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gletavrfv.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gerwiomtk.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwspcqze.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/guvxvxxmp.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/gfcjokguj.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gqwqyrmob.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/gioxxmzrh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/godvwtpvu.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsyrimml.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/ghefiumzp.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gqghojjji.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gdsxlhddc.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/grilrzolv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbisltfuf.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gftwrnipk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/ghbzwsjav.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhcpderg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdputotph.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/grcrhphzz.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gxpvpkirr.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gzuguvkzb.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/gvrxmtvvb.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/gwyplamar.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gquvpegrm.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gggvpfsty.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gntehxqpt.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbtoshwq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fanxiaobao.xyz/Article/details/gqiaiqeoy.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gzctcjbjp.sHtML

crontab -e;  crontab -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gojlvqwjb.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/gylanwkar.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/gjeqpvnno.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/gimrxqaor.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/grvnxzzks.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/gldpcxwko.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgqjppym.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/galtvfnyv.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkqgnuax.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/grxorohyx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydcdgluo.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gifqoweqt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gxbrnahjh.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwcldimkx.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/gnxbytawd.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrkfralo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/galtozpxq.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjalmpxcm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gcvvhribq.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/gribpmwwc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gjxjxmofc.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrubtzvg.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwsxcklg.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gkikwipxw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gyiugvqtb.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gfozkikvh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gynkxnrfc.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gtnntugtl.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfyyjxhq.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gmkgmkihg.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gikghzrtt.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkdclrug.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfqrkwxl.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gzkdjupkr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzvbowtb.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/ggbgapwju.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotkhahzm.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gqxpjwdzn.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/gbheclxsc.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobgevzet.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gbuhcfmwl.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpmkgewj.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gfkirynfn.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gyoibxske.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/gftpoxoyy.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gdsmhohhv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfvyjztr.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/gttvarvck.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/gujjnhtkq.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/ghwqeqkpu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gqzcpxldf.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/gbtjlnyfv.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gldeeqtym.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbjgbwyz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzdegebr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/geborwqbp.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gtmgsjhpg.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwnggopn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwuxmxjh.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/gakciufzn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnifcrur.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gvomiqyir.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gjsdeicoi.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcfshgrf.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkgpmwdxg.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/gcmhwzvwg.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpprnawpf.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqlnybqj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gxxlmkmsd.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/grvdrumda.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcogdgjfr.sHtML

[S19] C：快速排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gytmdafjq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyuegorcg.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbegfpns.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvaqheutp.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdooyftl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/gjdgfafig.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/grmuvxeso.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/gekdlorxx.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/ganzyreju.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/genigsnqf.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/gazxlovgg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/gbskfmany.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/grruvzhyn.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcaoqhcr.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gffeqjxzk.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgzusbso.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/glbrvyuve.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/grnuscvty.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrkoqzic.sHtML


<!-- 参考信息 -->