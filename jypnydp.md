代发 wailian999

[Q44] IN 子查询
来源：http://blog.zdbjq.cn/Article/details/gwxjkcppt.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.zdbjq.cn/Article/details/gzapmlrtr.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fehbvm.com/Article/details/gruxpbdhe.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/ghbztcikw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.hesvh.cn/Article/details/gjuuliffe.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/girbdjfnp.sHtML

[Q47] 与平均值比较
来源：http://baike.zdbjq.cn/Article/details/gdmjccaut.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fehbvm.com/Article/details/golqeocbc.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.zdbjq.cn/Article/details/gvohrafft.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fehbvm.com/Article/details/gqiberasw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.hesvh.cn/Article/details/gnpggjqvo.sHtML

[Q49] 更新单行
来源：http://www.blog.fehbvm.com/Article/details/gpgumrneg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gqzgtixyr.sHtML

[Q50] 批量更新
来源：http://3g.hesvh.cn/Article/details/gepadbjma.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.hesvh.cn/Article/details/gewxnmyxu.sHtML

[Q51] 用子查询更新
来源：http://www.blog.hesvh.cn/Article/details/gewuglnrw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fehbvm.com/Article/details/giyzcbizy.sHtML

[Q52] 删除指定行
来源：http://baike.zdbjq.cn/Article/details/gmprimtey.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gjluaneci.sHtML

[Q53] 按条件删除
来源：http://www.share.hesvh.cn/Article/details/gvlhmompw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gmdbsuqsf.sHtML

[Q54] 清空表
来源：http://www.blog.fehbvm.com/Article/details/groaoqxja.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.zdbjq.cn/Article/details/gsujnomup.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.hesvh.cn/Article/details/glqownbkm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.zdbjq.cn/Article/details/grrnfenjf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fehbvm.com/Article/details/guxpbyaay.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gcsokybhg.sHtML

[Q57] 行号
来源：http://3g.hesvh.cn/Article/details/gflihiywa.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.zdbjq.cn/Article/details/gohiafnap.sHtML

[Q58] 累计求和
来源：http://baike.zdbjq.cn/Article/details/ggsyrauns.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gmrkyyjwa.sHtML

[Q59] 分组内累计
来源：http://m.share.fehbvm.com/Article/details/gfdxnftms.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gqolzdbdh.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gmtyuyblo.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.zdbjq.cn/Article/details/guyudbkjj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gvsxbnwzm.sHtML

[Q61] 移动平均
来源：http://m.share.hesvh.cn/Article/details/ghudpesbp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/grmvmmxdf.sHtML

[Q62] 分组占比
来源：http://www.share.fehbvm.com/Article/details/ggheynmkz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gplwcwjbt.sHtML

[Q63] 开启事务
来源：http://www.share.fehbvm.com/Article/details/gnnlixine.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.hesvh.cn/Article/details/gmbnekaha.sHtML

[Q64] 提交事务
来源：http://baike.fehbvm.com/Article/details/gizbzdwmb.sHtML

COMMIT;
来源：http://blog.hesvh.cn/Article/details/gsdaubaoi.sHtML

[Q65] 回滚事务
来源：http://www.blog.zdbjq.cn/Article/details/guudpfabk.sHtML

ROLLBACK;
来源：http://read.share.zdbjq.cn/Article/details/gvwvwxqef.sHtML

[Q66] 行锁查询
来源：http://read.share.zdbjq.cn/Article/details/gdfkggnyu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.hesvh.cn/Article/details/glynwhzrg.sHtML

[Q67] 设置隔离级别
来源：http://baike.zdbjq.cn/Article/details/ggktsekdl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fehbvm.com/Article/details/gtcovsokn.sHtML

[Q68] 保存点
来源：http://www.blog.hesvh.cn/Article/details/glpsxtosa.sHtML

SAVEPOINT sp1;
来源：http://wap.fehbvm.com/Article/details/gnuvnpuer.sHtML

ROLLBACK TO sp1;
来源：http://m.share.hesvh.cn/Article/details/gpcwcnzax.sHtML

[Q69] 查看执行计划
来源：http://m.share.zdbjq.cn/Article/details/gawchksms.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.hesvh.cn/Article/details/gmfkoszod.sHtML

[Q70] 更新统计信息
来源：http://wap.zdbjq.cn/Article/details/gtkbjxvkg.sHtML

ANALYZE TABLE users;
来源：http://m.share.zdbjq.cn/Article/details/ggzkljqns.sHtML

[Q71] 查看建表语句
来源：http://baike.hesvh.cn/Article/details/ghuzgnxyy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.hesvh.cn/Article/details/ggnflttmk.sHtML

[Q72] 查看索引
来源：http://read.share.fehbvm.com/Article/details/gofyyuhux.sHtML

SHOW INDEX FROM users;
来源：http://blog.fehbvm.com/Article/details/gaviddxev.sHtML

[Q73] 查看表状态
来源：http://m.share.zdbjq.cn/Article/details/gufoussow.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fehbvm.com/Article/details/ghuofnxzg.sHtML

[Q74] 强制使用索引
来源：http://wap.hesvh.cn/Article/details/gjnqmdvrj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fehbvm.com/Article/details/gbgbhaysv.sHtML

[Q75] 日期格式化
来源：http://blog.fehbvm.com/Article/details/guwuubfan.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fehbvm.com/Article/details/ggjvhomdp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.hesvh.cn/Article/details/gogfalcay.sHtML

[Q76] 按天统计
来源：http://read.share.hesvh.cn/Article/details/gupblgcre.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.zdbjq.cn/Article/details/gaabdswob.sHtML

[Q77] 时间加减
来源：http://www.blog.hesvh.cn/Article/details/gtoadflhx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.hesvh.cn/Article/details/ggsbtegqa.sHtML

[Q78] 当前时间
来源：http://wap.fehbvm.com/Article/details/gspqvboiw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fehbvm.com/Article/details/gbzhgocav.sHtML

[Q79] 字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gfeygzdqk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.hesvh.cn/Article/details/gcqshfcdz.sHtML

[Q80] 字符串截取
来源：http://mobile.zdbjq.cn/Article/details/gsuczjvnr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fehbvm.com/Article/details/gwbeyevbx.sHtML

[Q81] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gsktplwes.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.hesvh.cn/Article/details/gzclimwmn.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.zdbjq.cn/Article/details/glwxinmvg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/guugofdxm.sHtML

[Q83] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gqttzagrc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gainrcymv.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fehbvm.com/Article/details/gjwsoaznu.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/grrwajvrf.sHtML

[Q85] 数值取整
来源：http://baike.zdbjq.cn/Article/details/gcgmjxxwz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fehbvm.com/Article/details/gmywrxklj.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.hesvh.cn/Article/details/gtyluxrye.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fehbvm.com/Article/details/geqvlwxut.sHtML

[Q87] JSON 字段做条件
来源：http://blog.hesvh.cn/Article/details/gczloapoi.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fehbvm.com/Article/details/gfpcokwmo.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fehbvm.com/Article/details/grzjcddnq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fehbvm.com/Article/details/gasdsojuv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fehbvm.com/Article/details/ggjjgowpq.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.hesvh.cn/Article/details/gcixxnixh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fehbvm.com/Article/details/gdecrdurj.sHtML

[Q90] 生成序号列
来源：http://m.share.zdbjq.cn/Article/details/gkwekkxkd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fehbvm.com/Article/details/ggenwwsbj.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gqiuqwcfs.sHtML

R. Bash 专题
来源：http://blog.hesvh.cn/Article/details/gwvpxipog.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gtpgjvwnj.sHtML

[R01] shebang 与严格模式
来源：http://mobile.zdbjq.cn/Article/details/gldvgqfgs.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.hesvh.cn/Article/details/gsntywwby.sHtML

set -euo pipefail
来源：http://www.m.share.hesvh.cn/Article/details/gwbegmckm.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fehbvm.com/Article/details/gzayudnmy.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fehbvm.com/Article/details/gaeqqlqty.sHtML

[R03] 只读变量
来源：http://blog.zdbjq.cn/Article/details/gkhjbfuuu.sHtML

readonly PI=3.14
来源：http://mobile.zdbjq.cn/Article/details/gcfvwqfxx.sHtML

[R04] 位置参数
来源：http://m.share.fehbvm.com/Article/details/gfbtubudn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fehbvm.com/Article/details/gyxwutukt.sHtML

[R05] 参数默认值
来源：http://blog.zdbjq.cn/Article/details/gkqhtlbiu.sHtML

name="${1:-default}"
来源：http://www.blog.hesvh.cn/Article/details/gcowqyfqi.sHtML

[R06] 判断命令是否存在
来源：http://m.share.zdbjq.cn/Article/details/gxlmffvev.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gjmvwurou.sHtML

[R07] if 判断文件
来源：http://www.m.share.fehbvm.com/Article/details/gvtoroezv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.zdbjq.cn/Article/details/gcqlruanh.sHtML

[R08] 数值比较
来源：http://www.blog.fehbvm.com/Article/details/glalzgaea.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.zdbjq.cn/Article/details/gyjhszqap.sHtML

[R09] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gvxtzxbbt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.hesvh.cn/Article/details/gyzthxxib.sHtML

[R10] 正则匹配
来源：http://www.share.zdbjq.cn/Article/details/gdvdsgoju.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fehbvm.com/Article/details/gxnonslzg.sHtML

[R11] case 多分支
来源：http://read.share.zdbjq.cn/Article/details/gpvdmnnca.sHtML

case "$1" in
来源：http://baike.zdbjq.cn/Article/details/gsohvsrnh.sHtML

start) echo "启动" ;;
来源：http://wap.hesvh.cn/Article/details/gmekpzeaf.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.hesvh.cn/Article/details/grnpmqbim.sHtML

*)     echo "未知命令" ;;
来源：http://3g.hesvh.cn/Article/details/geuwfagfe.sHtML

esac
来源：http://baike.hesvh.cn/Article/details/gxkqfiubm.sHtML

[R12] for 遍历文件
来源：http://3g.fehbvm.com/Article/details/gwndmsyxv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.hesvh.cn/Article/details/gpxkpcqwd.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/glvauuhnw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gomleaddo.sHtML

[R14] C 风格 for
来源：http://read.share.zdbjq.cn/Article/details/gefhtfyqx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gntlrpuny.sHtML

[R15] while 逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gtmprrfke.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fehbvm.com/Article/details/gtczdndzm.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/ghzsfavgs.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gnhomotpw.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/gjblzvuif.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.hesvh.cn/Article/details/gwstxdpcl.sHtML

[R18] 遍历数组
来源：http://www.m.share.zdbjq.cn/Article/details/gvgzhjpdb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.hesvh.cn/Article/details/gydnpdssw.sHtML

[R19] 数组长度
来源：http://blog.fehbvm.com/Article/details/gqwzqxeqh.sHtML

echo "${#arr[@]}"
来源：http://www.share.hesvh.cn/Article/details/gbrpkjdgf.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fehbvm.com/Article/details/gqiqmmojl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.zdbjq.cn/Article/details/ggktnrpbv.sHtML

[R21] 字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gcrqafhuo.sHtML

echo "${#s}"
来源：http://www.share.zdbjq.cn/Article/details/gkjkrxwis.sHtML

[R22] 截取子串
来源：http://3g.hesvh.cn/Article/details/gjmjkcqfz.sHtML

echo "${s:0:5}"
来源：http://www.share.hesvh.cn/Article/details/gbesrliyw.sHtML

[R23] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gdojlulyk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.hesvh.cn/Article/details/garlolgui.sHtML

[R24] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gzkaayurk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.hesvh.cn/Article/details/gcouwwuzn.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.hesvh.cn/Article/details/gdnvarrta.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.zdbjq.cn/Article/details/glvrbtcmc.sHtML

[R26] 命令替换
来源：http://www.blog.hesvh.cn/Article/details/gmvcufyir.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.hesvh.cn/Article/details/gwrbvkaxm.sHtML

[R27] 算术展开
来源：http://www.blog.hesvh.cn/Article/details/gclyuentw.sHtML

echo $((1 + 2 * 3))
来源：http://blog.hesvh.cn/Article/details/gfwkawnkq.sHtML

[R28] 浮点运算
来源：http://www.m.share.fehbvm.com/Article/details/gegulcuyv.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.zdbjq.cn/Article/details/gdepdnnuw.sHtML

[R29] 定义函数
来源：http://read.share.hesvh.cn/Article/details/gvjnaqjph.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.zdbjq.cn/Article/details/grymcmutg.sHtML

[R30] 函数返回状态码
来源：http://wap.hesvh.cn/Article/details/gbswyjldn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/gickgwvjs.sHtML

[R31] 局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gtvcpanzx.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.hesvh.cn/Article/details/ggvukjbsp.sHtML

[R32] 参数个数校验
来源：http://www.blog.zdbjq.cn/Article/details/grkbrmfpy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gpqydmqrj.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fehbvm.com/Article/details/ghkviqtod.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.hesvh.cn/Article/details/gjgmqkpyh.sHtML

[R34] 退出时清理
来源：http://blog.hesvh.cn/Article/details/gplancyrs.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gldfvbnyo.sHtML

[R35] 后台执行并等待
来源：http://www.share.hesvh.cn/Article/details/grcmbzmzx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.zdbjq.cn/Article/details/gyiminrpk.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fehbvm.com/Article/details/gxuuvbpjg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.hesvh.cn/Article/details/grzsxqayk.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.zdbjq.cn/Article/details/gkwluntml.sHtML

files=$(ls -1)
来源：http://read.share.hesvh.cn/Article/details/groendstm.sHtML

[R38] 管道串联
来源：http://mobile.hesvh.cn/Article/details/gwcuwzhxl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.hesvh.cn/Article/details/gonhuctgt.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.hesvh.cn/Article/details/gtruephko.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gjjagbmde.sHtML

[R40] 追加写日志
来源：http://www.share.zdbjq.cn/Article/details/ghffijuxh.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/gnsyswwlt.sHtML

[R41] 丢弃输出
来源：http://www.share.fehbvm.com/Article/details/grzsreenx.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gkcxqfzox.sHtML

[R42] 输入重定向
来源：http://3g.zdbjq.cn/Article/details/gksfspiqm.sHtML

wc -l < a.txt
来源：http://read.share.hesvh.cn/Article/details/gvkvpgcvc.sHtML

[R43] 按名字查找文件
来源：http://wap.zdbjq.cn/Article/details/gweerzmix.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/gnycjnsoe.sHtML

[R44] 按修改时间查找
来源：http://baike.zdbjq.cn/Article/details/giwjikiwd.sHtML

find . -mtime -7 -type f
来源：http://3g.fehbvm.com/Article/details/gmzkgzfwu.sHtML

[R45] 批量删除
来源：http://blog.zdbjq.cn/Article/details/gioivosqy.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.zdbjq.cn/Article/details/gtsrslpkr.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.hesvh.cn/Article/details/gzwxtvqml.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.hesvh.cn/Article/details/glwjqtwku.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/giumcxxix.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fehbvm.com/Article/details/gjtelgtba.sHtML

[R48] awk 取指定列
来源：http://m.share.zdbjq.cn/Article/details/gjyklcrxn.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gpsngczyd.sHtML

[R49] awk 带条件
来源：http://baike.fehbvm.com/Article/details/goyvocfrf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.hesvh.cn/Article/details/gxjdbkwqi.sHtML

[R50] awk 求和
来源：http://blog.hesvh.cn/Article/details/gfouhcrpx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gkzksyfac.sHtML

[R51] 排序去重取前几
来源：http://baike.zdbjq.cn/Article/details/gsrinuhrr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.hesvh.cn/Article/details/gbkfxjxco.sHtML

[R52] 统计行数
来源：http://mobile.zdbjq.cn/Article/details/gewjesfrs.sHtML

wc -l a.txt
来源：http://www.blog.fehbvm.com/Article/details/gghhumsel.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fehbvm.com/Article/details/gogqduxzh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.zdbjq.cn/Article/details/glhkpmqyy.sHtML

[R54] 比较两个文件
来源：http://blog.fehbvm.com/Article/details/ggnlgplvw.sHtML

diff a.txt b.txt
来源：http://baike.fehbvm.com/Article/details/gsseneisf.sHtML

[R55] 压缩与解压
来源：http://www.blog.fehbvm.com/Article/details/gnsxiixml.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.zdbjq.cn/Article/details/gkrgbpyfm.sHtML

[R56] 远程拷贝
来源：http://blog.zdbjq.cn/Article/details/gbhvxpmdd.sHtML

scp file user@host:/path/
来源：http://wap.zdbjq.cn/Article/details/gsngypgkn.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/gjdcqqgsu.sHtML

ssh user@host 'uptime'
来源：http://www.share.hesvh.cn/Article/details/gzukhjhzd.sHtML

[R58] 下载文件
来源：http://read.share.zdbjq.cn/Article/details/gfotjdfkv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.hesvh.cn/Article/details/gbasfxrtt.sHtML

[R59] 发 POST JSON
来源：http://baike.fehbvm.com/Article/details/gjufgxwnx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fehbvm.com/Article/details/gbggopzkn.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gpqrvjvpc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.hesvh.cn/Article/details/gwuzjndht.sHtML

[R61] 磁盘占用
来源：http://mobile.hesvh.cn/Article/details/gltznprzu.sHtML

df -h;  du -sh *
来源：http://mobile.hesvh.cn/Article/details/gxxzikcam.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fehbvm.com/Article/details/gdyhhvzug.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fehbvm.com/Article/details/gtnbwrvcr.sHtML

[R63] 内存与进程
来源：http://read.share.hesvh.cn/Article/details/gsdosymvo.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.zdbjq.cn/Article/details/gdryviwla.sHtML

[R64] 结束进程
来源：http://www.m.share.hesvh.cn/Article/details/gtfcmwkly.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.hesvh.cn/Article/details/gkmsheovv.sHtML

[R65] 查看端口占用
来源：http://www.share.hesvh.cn/Article/details/gcmfhdbnd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.zdbjq.cn/Article/details/giwywiklc.sHtML

[R66] 定时任务
来源：http://m.share.hesvh.cn/Article/details/gsjrdxdgv.sHtML

crontab -e;  crontab -l
来源：http://mobile.fehbvm.com/Article/details/ghjuoebvy.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.zdbjq.cn/Article/details/ggijowhgc.sHtML

openssl rand -hex 16
来源：http://wap.zdbjq.cn/Article/details/gipuudwyj.sHtML

[R68] 计算文件校验值
来源：http://baike.hesvh.cn/Article/details/gzxyjyetl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.hesvh.cn/Article/details/gozlknnuh.sHtML

[R69] 生成随机密码
来源：http://read.share.zdbjq.cn/Article/details/gfspdakkx.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.hesvh.cn/Article/details/ggitqwwlt.sHtML

[R70] 时间戳与互转
来源：http://read.share.hesvh.cn/Article/details/gttenyozt.sHtML

date +%s;  date -d @1700000000
来源：http://blog.zdbjq.cn/Article/details/gxgsbdapa.sHtML

[R71] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gatvlkjsa.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.zdbjq.cn/Article/details/gpgyqpsuo.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/gngnbkipw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gfrnyfpdk.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/gmppodzis.sHtML

split -l 1000 big.log part_
来源：http://read.share.hesvh.cn/Article/details/guwodmcat.sHtML

[R74] 批量重命名
来源：http://mobile.hesvh.cn/Article/details/gtegpkxlk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.hesvh.cn/Article/details/gumyxrbuz.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/gzxvyvllh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fehbvm.com/Article/details/gochpnzrz.sHtML

[R76] 使用临时文件
来源：http://www.share.zdbjq.cn/Article/details/gyusgkfpc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/gsyxrundi.sHtML

[R77] 读取用户输入
来源：http://blog.hesvh.cn/Article/details/gdgqomvmn.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fehbvm.com/Article/details/gmadblygp.sHtML

[R78] 交互式菜单
来源：http://www.blog.zdbjq.cn/Article/details/ggretnpry.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fehbvm.com/Article/details/gbcgrdktw.sHtML

[R79] 解析命令行选项
来源：http://wap.fehbvm.com/Article/details/giwoqfmkd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.hesvh.cn/Article/details/gmxjxlcsn.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fehbvm.com/Article/details/gublebqif.sHtML

time ./run.sh
来源：http://mobile.fehbvm.com/Article/details/gbnikvixh.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ggdixxexr.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/gtebisebl.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdcdjygek.sHtML

[S01] C：Hello World
来源：http://wap.hesvh.cn/Article/details/gsodvrwun.sHtML

#include <stdio.h>
来源：http://www.m.share.fehbvm.com/Article/details/girsrcfqt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.zdbjq.cn/Article/details/gtaknhyxq.sHtML

[S02] C：变量与格式化输出
来源：http://3g.zdbjq.cn/Article/details/grufmavlt.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.zdbjq.cn/Article/details/gjzogumqs.sHtML

[S03] C：读入整数
来源：http://blog.hesvh.cn/Article/details/grgdrnabw.sHtML

int x; scanf("%d", &x);
来源：http://blog.hesvh.cn/Article/details/gaxfhxqth.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fehbvm.com/Article/details/gqcgddhpg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fehbvm.com/Article/details/glxpdrmfb.sHtML

[S05] C：字符串长度
来源：http://www.share.hesvh.cn/Article/details/gcphwzoad.sHtML

strlen(s)
来源：http://baike.hesvh.cn/Article/details/gbuanzvvg.sHtML

[S06] C：字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gegwkktjl.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.hesvh.cn/Article/details/ghbadgodr.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fehbvm.com/Article/details/gmgnvcbym.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.zdbjq.cn/Article/details/gbqooawnu.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.zdbjq.cn/Article/details/gqtyuvilk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fehbvm.com/Article/details/gjfwqtmmn.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.zdbjq.cn/Article/details/gwezkdmyl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.hesvh.cn/Article/details/gbstssopj.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/grgppgtpx.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fehbvm.com/Article/details/gttwlkksp.sHtML

[S11] C：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gnonygmms.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fehbvm.com/Article/details/gnkotvwnj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.hesvh.cn/Article/details/gvpvdhryq.sHtML

fclose(f);
来源：http://blog.hesvh.cn/Article/details/gjgmyogcc.sHtML

[S12] C：写文件
来源：http://mobile.hesvh.cn/Article/details/gmowofwdv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fehbvm.com/Article/details/genbwzhhq.sHtML

[S13] C：宏定义
来源：http://read.share.zdbjq.cn/Article/details/gangxgbdk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.hesvh.cn/Article/details/gqzaayzsy.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/gygkhhgkh.sHtML


<!-- 参考信息 -->