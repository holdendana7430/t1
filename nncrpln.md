代发 wailian999

[Q48] CTE 公用表表达式
来源：http://baike.fehbvm.com/Article/details/gfduimhuk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fehbvm.com/Article/details/gaqtqxwgx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fehbvm.com/Article/details/gislpizjw.sHtML

[Q49] 更新单行
来源：http://www.share.fehbvm.com/Article/details/gbxxucgsp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gcwgtshbv.sHtML

[Q50] 批量更新
来源：http://www.blog.zdbjq.cn/Article/details/gnzpwnkak.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fehbvm.com/Article/details/gmmhjgjsk.sHtML

[Q51] 用子查询更新
来源：http://read.share.hesvh.cn/Article/details/gsebuztfz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.zdbjq.cn/Article/details/ghgztwrtv.sHtML

[Q52] 删除指定行
来源：http://www.blog.zdbjq.cn/Article/details/gjtrptayv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/ghwrsyfpe.sHtML

[Q53] 按条件删除
来源：http://wap.fehbvm.com/Article/details/gjwamxprv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.zdbjq.cn/Article/details/ghhqtssod.sHtML

[Q54] 清空表
来源：http://baike.zdbjq.cn/Article/details/grbfudkjs.sHtML

TRUNCATE TABLE logs;
来源：http://blog.zdbjq.cn/Article/details/geszrpaih.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fehbvm.com/Article/details/gckonuwmv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.hesvh.cn/Article/details/gvqjdrogm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.zdbjq.cn/Article/details/giqmbbgsv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fehbvm.com/Article/details/gyqmxslfx.sHtML

[Q57] 行号
来源：http://www.share.zdbjq.cn/Article/details/guiuudqzu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fehbvm.com/Article/details/gwslgapmh.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/gzfxydwln.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fehbvm.com/Article/details/guodjhoca.sHtML

[Q59] 分组内累计
来源：http://www.blog.hesvh.cn/Article/details/gjaaailoe.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/ghbfmyoxv.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.zdbjq.cn/Article/details/gcistfwnn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fehbvm.com/Article/details/ghmjrawwa.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gnqnqrnjf.sHtML

[Q61] 移动平均
来源：http://mobile.fehbvm.com/Article/details/gxwhcqsko.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gcmgngxnf.sHtML

[Q62] 分组占比
来源：http://wap.hesvh.cn/Article/details/gtsxyfiaz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/ghzhvcxvc.sHtML

[Q63] 开启事务
来源：http://mobile.hesvh.cn/Article/details/gsbhehoor.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fehbvm.com/Article/details/gtwumdetz.sHtML

[Q64] 提交事务
来源：http://www.blog.fehbvm.com/Article/details/gltermdsu.sHtML

COMMIT;
来源：http://mobile.fehbvm.com/Article/details/gqiwcplfb.sHtML

[Q65] 回滚事务
来源：http://baike.fehbvm.com/Article/details/gkomwjaee.sHtML

ROLLBACK;
来源：http://read.share.fehbvm.com/Article/details/gkwyqgmzv.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/gdaedfmyd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.zdbjq.cn/Article/details/gzhoapeas.sHtML

[Q67] 设置隔离级别
来源：http://mobile.zdbjq.cn/Article/details/giwvnxhcj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fehbvm.com/Article/details/gwczuesnk.sHtML

[Q68] 保存点
来源：http://wap.fehbvm.com/Article/details/goansvyub.sHtML

SAVEPOINT sp1;
来源：http://www.share.fehbvm.com/Article/details/gmnocijeb.sHtML

ROLLBACK TO sp1;
来源：http://baike.hesvh.cn/Article/details/gbfqkjsat.sHtML

[Q69] 查看执行计划
来源：http://wap.hesvh.cn/Article/details/gmomjcwvg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.hesvh.cn/Article/details/goelkcjxl.sHtML

[Q70] 更新统计信息
来源：http://m.share.fehbvm.com/Article/details/gxrwnhymh.sHtML

ANALYZE TABLE users;
来源：http://blog.fehbvm.com/Article/details/guthsctfu.sHtML

[Q71] 查看建表语句
来源：http://mobile.zdbjq.cn/Article/details/gfndamlwr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.hesvh.cn/Article/details/gxkohefsh.sHtML

[Q72] 查看索引
来源：http://www.blog.hesvh.cn/Article/details/gwyqvluik.sHtML

SHOW INDEX FROM users;
来源：http://baike.zdbjq.cn/Article/details/gcqlulatg.sHtML

[Q73] 查看表状态
来源：http://mobile.zdbjq.cn/Article/details/gztwzbmvb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fehbvm.com/Article/details/gnprmpnlj.sHtML

[Q74] 强制使用索引
来源：http://read.share.hesvh.cn/Article/details/gtamglddz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.hesvh.cn/Article/details/gosvisrow.sHtML

[Q75] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gbuhylzlk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gbswcjwwe.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fehbvm.com/Article/details/giqqzrprz.sHtML

[Q76] 按天统计
来源：http://www.blog.fehbvm.com/Article/details/gauusduwx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.hesvh.cn/Article/details/gxakdqbkw.sHtML

[Q77] 时间加减
来源：http://www.blog.fehbvm.com/Article/details/gmuflniup.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.zdbjq.cn/Article/details/gyczfpykr.sHtML

[Q78] 当前时间
来源：http://blog.zdbjq.cn/Article/details/gjvlilqzm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fehbvm.com/Article/details/guqvajpdt.sHtML

[Q79] 字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gzwcpoojj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.hesvh.cn/Article/details/gmeavrfmw.sHtML

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/guajwfath.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fehbvm.com/Article/details/gfiuqhphc.sHtML

[Q81] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gitfxlkgc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fehbvm.com/Article/details/ghfejbkzk.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.hesvh.cn/Article/details/gqapdghjs.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gxvdhbhng.sHtML

[Q83] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gfkbmmidh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/goqpjsynv.sHtML

[Q84] 去除首尾空格
来源：http://baike.fehbvm.com/Article/details/gvhnydbaq.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/ggaklwhpa.sHtML

[Q85] 数值取整
来源：http://3g.hesvh.cn/Article/details/gimhsfzgs.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.zdbjq.cn/Article/details/gxkheurjz.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.hesvh.cn/Article/details/gxldrapxt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fehbvm.com/Article/details/gqfaprpko.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.hesvh.cn/Article/details/gppbhzvss.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.zdbjq.cn/Article/details/gjvwmzyfh.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fehbvm.com/Article/details/gwxwhblkq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fehbvm.com/Article/details/gvfnjpwux.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fehbvm.com/Article/details/gmzzayjec.sHtML

[Q89] 判断表是否存在
来源：http://wap.hesvh.cn/Article/details/gexsycgqb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.zdbjq.cn/Article/details/gorxggwvs.sHtML

[Q90] 生成序号列
来源：http://wap.hesvh.cn/Article/details/ghamfvyro.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.zdbjq.cn/Article/details/gssndlund.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gywdugzxa.sHtML

R. Bash 专题
来源：http://blog.hesvh.cn/Article/details/gjpqgaked.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/govqgdgrk.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fehbvm.com/Article/details/gxqunhnwa.sHtML

#!/usr/bin/env bash
来源：http://www.share.zdbjq.cn/Article/details/gmupvdwel.sHtML

set -euo pipefail
来源：http://baike.fehbvm.com/Article/details/gsgmekurk.sHtML

[R02] 变量赋值与使用
来源：http://3g.hesvh.cn/Article/details/ghszllhel.sHtML

name="Tom"; echo "$name"
来源：http://wap.hesvh.cn/Article/details/gitxjidlj.sHtML

[R03] 只读变量
来源：http://www.m.share.zdbjq.cn/Article/details/gayqtifbu.sHtML

readonly PI=3.14
来源：http://3g.hesvh.cn/Article/details/gwpcxheyz.sHtML

[R04] 位置参数
来源：http://mobile.hesvh.cn/Article/details/goozffbtf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fehbvm.com/Article/details/gxirpyjzt.sHtML

[R05] 参数默认值
来源：http://www.m.share.hesvh.cn/Article/details/grqcsqxad.sHtML

name="${1:-default}"
来源：http://baike.zdbjq.cn/Article/details/grtubljpa.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fehbvm.com/Article/details/gwbevkqfb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gscmialrz.sHtML

[R07] if 判断文件
来源：http://blog.zdbjq.cn/Article/details/gofpdxqje.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.zdbjq.cn/Article/details/gxhiklmdu.sHtML

[R08] 数值比较
来源：http://read.share.hesvh.cn/Article/details/gohatxjhk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.hesvh.cn/Article/details/gojtolhse.sHtML

[R09] 字符串比较
来源：http://mobile.hesvh.cn/Article/details/guemxirux.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.zdbjq.cn/Article/details/gddhnwiqu.sHtML

[R10] 正则匹配
来源：http://mobile.zdbjq.cn/Article/details/gutefwtfz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.hesvh.cn/Article/details/gnglxwgrg.sHtML

[R11] case 多分支
来源：http://3g.hesvh.cn/Article/details/gxmqdnzbq.sHtML

case "$1" in
来源：http://www.share.hesvh.cn/Article/details/gzdykohxy.sHtML

start) echo "启动" ;;
来源：http://wap.zdbjq.cn/Article/details/gwxcivymr.sHtML

stop)  echo "停止" ;;
来源：http://www.share.zdbjq.cn/Article/details/gzudhohfv.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.zdbjq.cn/Article/details/gvsvhsvab.sHtML

esac
来源：http://wap.fehbvm.com/Article/details/gwhxxeomv.sHtML

[R12] for 遍历文件
来源：http://www.blog.hesvh.cn/Article/details/gqjoydopt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.zdbjq.cn/Article/details/gmyhfgqhq.sHtML

[R13] for 计数循环
来源：http://3g.fehbvm.com/Article/details/gfztzgacr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gacusuwzj.sHtML

[R14] C 风格 for
来源：http://m.share.hesvh.cn/Article/details/gjbaanuzi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gwndcwxkw.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gnscbstha.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.hesvh.cn/Article/details/ghkphyeox.sHtML

[R16] until 等待条件
来源：http://m.share.hesvh.cn/Article/details/gmujizine.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gbpmuffqv.sHtML

[R17] 数组定义与取值
来源：http://www.share.hesvh.cn/Article/details/giozemfuf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gjdekxfmg.sHtML

[R18] 遍历数组
来源：http://blog.hesvh.cn/Article/details/gajvbegcl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.zdbjq.cn/Article/details/geviaazdo.sHtML

[R19] 数组长度
来源：http://www.share.hesvh.cn/Article/details/geixwecpj.sHtML

echo "${#arr[@]}"
来源：http://blog.fehbvm.com/Article/details/glzyyapma.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fehbvm.com/Article/details/gqrlpixro.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/gcddktrna.sHtML

[R21] 字符串长度
来源：http://blog.hesvh.cn/Article/details/guzpvaeuc.sHtML

echo "${#s}"
来源：http://read.share.hesvh.cn/Article/details/gtbkwuyuh.sHtML

[R22] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gzumsyivt.sHtML

echo "${s:0:5}"
来源：http://read.share.fehbvm.com/Article/details/goiignajo.sHtML

[R23] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gedxodnou.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.hesvh.cn/Article/details/gyjhbxwnq.sHtML

[R24] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gaouwhxgj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fehbvm.com/Article/details/gggdyurpi.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.zdbjq.cn/Article/details/gmgqlleer.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.hesvh.cn/Article/details/gmtmtilwg.sHtML

[R26] 命令替换
来源：http://www.m.share.hesvh.cn/Article/details/grepynixi.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.zdbjq.cn/Article/details/gkrixcmio.sHtML

[R27] 算术展开
来源：http://www.share.zdbjq.cn/Article/details/gkugkvbmi.sHtML

echo $((1 + 2 * 3))
来源：http://baike.hesvh.cn/Article/details/gnqmosvpn.sHtML

[R28] 浮点运算
来源：http://3g.fehbvm.com/Article/details/gwtbuhhha.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fehbvm.com/Article/details/garynlhsr.sHtML

[R29] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/gxkywwhlm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.hesvh.cn/Article/details/gnyotgpnk.sHtML

[R30] 函数返回状态码
来源：http://wap.zdbjq.cn/Article/details/gkuqkoozn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.zdbjq.cn/Article/details/gzozsfoxt.sHtML

[R31] 局部变量
来源：http://wap.hesvh.cn/Article/details/gzvlyhsip.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.hesvh.cn/Article/details/gsgqibjmw.sHtML

[R32] 参数个数校验
来源：http://baike.hesvh.cn/Article/details/ghrmbswyo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/ggzmficcd.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fehbvm.com/Article/details/gdqcejnau.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.hesvh.cn/Article/details/gdixtyewb.sHtML

[R34] 退出时清理
来源：http://www.share.fehbvm.com/Article/details/gwteycget.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gfvnfexha.sHtML

[R35] 后台执行并等待
来源：http://blog.hesvh.cn/Article/details/gpokreuzx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.zdbjq.cn/Article/details/gcswmtvzu.sHtML

[R36] 并发执行多个任务
来源：http://baike.hesvh.cn/Article/details/grhvxwnci.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fehbvm.com/Article/details/gdmjvaisf.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fehbvm.com/Article/details/glhzctqvb.sHtML

files=$(ls -1)
来源：http://blog.zdbjq.cn/Article/details/gtxtrtlnc.sHtML

[R38] 管道串联
来源：http://mobile.zdbjq.cn/Article/details/gcufemdzw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.hesvh.cn/Article/details/gndotqobg.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.zdbjq.cn/Article/details/geynrdbjr.sHtML

cmd > out.log 2>&1
来源：http://baike.fehbvm.com/Article/details/gkqlhhgbw.sHtML

[R40] 追加写日志
来源：http://m.share.zdbjq.cn/Article/details/gcdmefcpg.sHtML

echo "log" >> out.log
来源：http://baike.fehbvm.com/Article/details/gkzxwdwbw.sHtML

[R41] 丢弃输出
来源：http://blog.fehbvm.com/Article/details/gamlzozwk.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gcbbflfjw.sHtML

[R42] 输入重定向
来源：http://m.share.hesvh.cn/Article/details/gnjfanfda.sHtML

wc -l < a.txt
来源：http://www.blog.hesvh.cn/Article/details/gmowecbhz.sHtML

[R43] 按名字查找文件
来源：http://www.share.zdbjq.cn/Article/details/gxkqigmye.sHtML

find . -name "*.log" -type f
来源：http://www.share.fehbvm.com/Article/details/gmhxmqoio.sHtML

[R44] 按修改时间查找
来源：http://3g.fehbvm.com/Article/details/ggnhxdcxb.sHtML

find . -mtime -7 -type f
来源：http://mobile.zdbjq.cn/Article/details/gyavktwfb.sHtML

[R45] 批量删除
来源：http://baike.zdbjq.cn/Article/details/gqkmlzium.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fehbvm.com/Article/details/gezwjywhz.sHtML

[R46] 递归替换文件内容
来源：http://blog.zdbjq.cn/Article/details/gzwfhwcbv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.hesvh.cn/Article/details/ghdgeqjic.sHtML

[R47] sed 单行替换
来源：http://www.share.fehbvm.com/Article/details/gjexllrfu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gnwdrhqqz.sHtML

[R48] awk 取指定列
来源：http://www.blog.fehbvm.com/Article/details/gttzbqczb.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gvdtjabrk.sHtML

[R49] awk 带条件
来源：http://www.m.share.zdbjq.cn/Article/details/ghzlogbwe.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.hesvh.cn/Article/details/gywrdogsr.sHtML

[R50] awk 求和
来源：http://3g.zdbjq.cn/Article/details/ghbkfsjpl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/ghwklnnvl.sHtML

[R51] 排序去重取前几
来源：http://mobile.fehbvm.com/Article/details/gydvtvbgi.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.hesvh.cn/Article/details/godjeybfl.sHtML

[R52] 统计行数
来源：http://wap.zdbjq.cn/Article/details/gowsowlaw.sHtML

wc -l a.txt
来源：http://www.blog.fehbvm.com/Article/details/gemonhxmk.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.hesvh.cn/Article/details/gqchkrwdt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fehbvm.com/Article/details/gygbpdbkn.sHtML

[R54] 比较两个文件
来源：http://www.share.zdbjq.cn/Article/details/gqgkpfemz.sHtML

diff a.txt b.txt
来源：http://www.blog.hesvh.cn/Article/details/ghprsqgzm.sHtML

[R55] 压缩与解压
来源：http://mobile.fehbvm.com/Article/details/gzncrbkrz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.hesvh.cn/Article/details/gvvzrdccs.sHtML

[R56] 远程拷贝
来源：http://wap.zdbjq.cn/Article/details/gdcjhdomd.sHtML

scp file user@host:/path/
来源：http://m.share.hesvh.cn/Article/details/gmyfatvdk.sHtML

[R57] 远程执行命令
来源：http://www.m.share.zdbjq.cn/Article/details/goaohsqyt.sHtML

ssh user@host 'uptime'
来源：http://wap.hesvh.cn/Article/details/gvakbamse.sHtML

[R58] 下载文件
来源：http://blog.fehbvm.com/Article/details/gfkyoliah.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fehbvm.com/Article/details/gurydfiwh.sHtML

[R59] 发 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gqqmggxxt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.zdbjq.cn/Article/details/gmvzemjzp.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gstnoyakw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fehbvm.com/Article/details/ghpwmeckc.sHtML

[R61] 磁盘占用
来源：http://www.m.share.zdbjq.cn/Article/details/gmyilgbxy.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/gjjkbmmfv.sHtML

[R62] 找最占空间的文件
来源：http://3g.fehbvm.com/Article/details/gpzfvfkfr.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fehbvm.com/Article/details/gbycmzxdg.sHtML

[R63] 内存与进程
来源：http://wap.hesvh.cn/Article/details/gjzbxkxla.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fehbvm.com/Article/details/gretelpuw.sHtML

[R64] 结束进程
来源：http://blog.hesvh.cn/Article/details/gvczyfsxc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.hesvh.cn/Article/details/ggabsfpxf.sHtML

[R65] 查看端口占用
来源：http://blog.fehbvm.com/Article/details/gsowhiczk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fehbvm.com/Article/details/ghasafjyv.sHtML

[R66] 定时任务
来源：http://m.share.fehbvm.com/Article/details/gwunzcrxw.sHtML

crontab -e;  crontab -l
来源：http://baike.hesvh.cn/Article/details/gasjrgxbv.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/gtcykiseo.sHtML

openssl rand -hex 16
来源：http://read.share.zdbjq.cn/Article/details/gfkgheick.sHtML

[R68] 计算文件校验值
来源：http://blog.hesvh.cn/Article/details/gbxhdmtcu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/gfwotmqwm.sHtML

[R69] 生成随机密码
来源：http://wap.fehbvm.com/Article/details/gloemifyy.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.zdbjq.cn/Article/details/gepckutjz.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fehbvm.com/Article/details/gviojdldd.sHtML

date +%s;  date -d @1700000000
来源：http://blog.hesvh.cn/Article/details/gdvpzabca.sHtML

[R71] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gfixrtvsr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.zdbjq.cn/Article/details/gysljfpwf.sHtML

[R72] 等待端口就绪
来源：http://3g.zdbjq.cn/Article/details/gkatkpoxj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gshkqxemo.sHtML

[R73] 分割大日志
来源：http://www.blog.fehbvm.com/Article/details/gccfohimy.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fehbvm.com/Article/details/goejzspgy.sHtML

[R74] 批量重命名
来源：http://m.share.zdbjq.cn/Article/details/ghxfjkzlc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.zdbjq.cn/Article/details/gicpwbzby.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gjxnyihsq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.hesvh.cn/Article/details/gvtqshspe.sHtML

[R76] 使用临时文件
来源：http://www.share.zdbjq.cn/Article/details/gvfjqsiuf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gnvhcywgg.sHtML

[R77] 读取用户输入
来源：http://blog.zdbjq.cn/Article/details/gtwtipyup.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fehbvm.com/Article/details/gtqhewyfr.sHtML

[R78] 交互式菜单
来源：http://wap.zdbjq.cn/Article/details/guxgibkfk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/gwoxeqlwb.sHtML

[R79] 解析命令行选项
来源：http://baike.hesvh.cn/Article/details/gorcdanel.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.zdbjq.cn/Article/details/gbyoyzdji.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fehbvm.com/Article/details/gyigwygpw.sHtML

time ./run.sh
来源：http://baike.hesvh.cn/Article/details/goeujqjpo.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gksayozyz.sHtML

S. C / C++ 专题
来源：http://baike.fehbvm.com/Article/details/gnoncdsqz.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gkxymywmi.sHtML

[S01] C：Hello World
来源：http://baike.fehbvm.com/Article/details/gjvjznkam.sHtML

#include <stdio.h>
来源：http://read.share.fehbvm.com/Article/details/gkczsmezv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.hesvh.cn/Article/details/gywqxehfo.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.hesvh.cn/Article/details/gfhcfgvjr.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.hesvh.cn/Article/details/gvggsftpe.sHtML

[S03] C：读入整数
来源：http://wap.fehbvm.com/Article/details/gazktflmo.sHtML

int x; scanf("%d", &x);
来源：http://wap.hesvh.cn/Article/details/gobvblshx.sHtML

[S04] C：字符串复制
来源：http://blog.fehbvm.com/Article/details/gwpeqbysf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.zdbjq.cn/Article/details/gctpxvetq.sHtML

[S05] C：字符串长度
来源：http://m.share.hesvh.cn/Article/details/gkbrdaodl.sHtML

strlen(s)
来源：http://m.share.hesvh.cn/Article/details/gbeyznnzv.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/gomsyrtvu.sHtML

strcmp(a, b) == 0
来源：http://www.share.fehbvm.com/Article/details/giuarnqzu.sHtML

[S07] C：数组遍历求和
来源：http://blog.hesvh.cn/Article/details/gtbdieiid.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fehbvm.com/Article/details/gvjuztorp.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.zdbjq.cn/Article/details/glhqvlksr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.hesvh.cn/Article/details/gutruqvdm.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fehbvm.com/Article/details/ggpprpwdt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fehbvm.com/Article/details/grbtoqqbl.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fehbvm.com/Article/details/givmcxifb.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.zdbjq.cn/Article/details/grdwfkyxl.sHtML

[S11] C：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gfaturizq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.hesvh.cn/Article/details/gzegczxzx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gvyzcigmf.sHtML

fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gubpfeyqu.sHtML

[S12] C：写文件
来源：http://read.share.zdbjq.cn/Article/details/gcnemnvyw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gpbzimkys.sHtML

[S13] C：宏定义
来源：http://wap.fehbvm.com/Article/details/grqjghtrp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fehbvm.com/Article/details/geomwzhvm.sHtML

[S14] C：枚举
来源：http://m.share.fehbvm.com/Article/details/glpcnzgqe.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.zdbjq.cn/Article/details/ggiuqseff.sHtML

[S15] C：类型转换
来源：http://blog.hesvh.cn/Article/details/grdhcngdg.sHtML

(double) a / b
来源：http://www.share.zdbjq.cn/Article/details/gktzixywo.sHtML

[S16] C：位操作置位
来源：http://blog.fehbvm.com/Article/details/gukusdgvk.sHtML

x |= (1 << 3);
来源：http://wap.hesvh.cn/Article/details/gjylegaeg.sHtML

[S17] C：安全拼接字符串
来源：http://baike.hesvh.cn/Article/details/giexbdkal.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/gcccidimh.sHtML

[S18] C：命令行参数
来源：http://baike.zdbjq.cn/Article/details/gihyobrlo.sHtML


<!-- 参考信息 -->