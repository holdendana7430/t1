代发 wailian999

[Q44] IN 子查询
来源：http://3g.fehbvm.com/Article/details/gevolzcpp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.hesvh.cn/Article/details/gjagexbot.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.hesvh.cn/Article/details/gkjixxict.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/grvygvhgg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.zdbjq.cn/Article/details/gyeovxrnq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gdchbkdut.sHtML

[Q47] 与平均值比较
来源：http://www.share.hesvh.cn/Article/details/gxzxdrqkv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.zdbjq.cn/Article/details/gqzozihml.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.hesvh.cn/Article/details/ghfmeqrst.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fehbvm.com/Article/details/gelfrgask.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fehbvm.com/Article/details/gsvqkxrxg.sHtML

[Q49] 更新单行
来源：http://wap.fehbvm.com/Article/details/gflgqcqvi.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gldhpxwhs.sHtML

[Q50] 批量更新
来源：http://wap.fehbvm.com/Article/details/gdouiosrz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gylufzuoe.sHtML

[Q51] 用子查询更新
来源：http://read.share.fehbvm.com/Article/details/gpjokofbl.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gjwbxiiqd.sHtML

[Q52] 删除指定行
来源：http://www.m.share.zdbjq.cn/Article/details/gnxwfbnwm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gaeqkjxnj.sHtML

[Q53] 按条件删除
来源：http://mobile.hesvh.cn/Article/details/gnmexioab.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/ggjduuqao.sHtML

[Q54] 清空表
来源：http://www.m.share.zdbjq.cn/Article/details/gespuxfbl.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fehbvm.com/Article/details/gagacysas.sHtML

[Q55] 排名（并列占位）
来源：http://3g.zdbjq.cn/Article/details/gvnzuonse.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.hesvh.cn/Article/details/ggadgojnc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.zdbjq.cn/Article/details/gjmriqqtd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fehbvm.com/Article/details/gwsbwntgm.sHtML

[Q57] 行号
来源：http://3g.fehbvm.com/Article/details/ggksfotfh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fehbvm.com/Article/details/gbfxqfncn.sHtML

[Q58] 累计求和
来源：http://mobile.hesvh.cn/Article/details/gcthwkuei.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.hesvh.cn/Article/details/gckyycesn.sHtML

[Q59] 分组内累计
来源：http://3g.fehbvm.com/Article/details/gjwxyiupt.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gnlvwqhdv.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.zdbjq.cn/Article/details/gecxbcevl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.hesvh.cn/Article/details/ghydsogmh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gymwwlxyf.sHtML

[Q61] 移动平均
来源：http://www.blog.zdbjq.cn/Article/details/guyhppbms.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gjwgzqkfd.sHtML

[Q62] 分组占比
来源：http://www.share.fehbvm.com/Article/details/gzqsbqofw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gecuympkv.sHtML

[Q63] 开启事务
来源：http://www.m.share.zdbjq.cn/Article/details/giqnweioo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.zdbjq.cn/Article/details/gbkpkskdf.sHtML

[Q64] 提交事务
来源：http://www.m.share.hesvh.cn/Article/details/gdyfpzoxx.sHtML

COMMIT;
来源：http://m.share.hesvh.cn/Article/details/gpeiicuqm.sHtML

[Q65] 回滚事务
来源：http://mobile.fehbvm.com/Article/details/ghsvwaytt.sHtML

ROLLBACK;
来源：http://wap.fehbvm.com/Article/details/gnyyqpzrj.sHtML

[Q66] 行锁查询
来源：http://wap.fehbvm.com/Article/details/gawiragcn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.zdbjq.cn/Article/details/gvcovfebs.sHtML

[Q67] 设置隔离级别
来源：http://www.share.zdbjq.cn/Article/details/gjpeqbfik.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.zdbjq.cn/Article/details/govwziarz.sHtML

[Q68] 保存点
来源：http://blog.hesvh.cn/Article/details/gdrqgttud.sHtML

SAVEPOINT sp1;
来源：http://m.share.fehbvm.com/Article/details/gqfvbarjr.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fehbvm.com/Article/details/gkicoydjt.sHtML

[Q69] 查看执行计划
来源：http://www.blog.hesvh.cn/Article/details/gmhxngumg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.hesvh.cn/Article/details/gegjvvtgc.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.zdbjq.cn/Article/details/gophfztai.sHtML

ANALYZE TABLE users;
来源：http://m.share.hesvh.cn/Article/details/gtqnpjizd.sHtML

[Q71] 查看建表语句
来源：http://www.share.hesvh.cn/Article/details/gxichmxok.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fehbvm.com/Article/details/ghdhwodat.sHtML

[Q72] 查看索引
来源：http://3g.hesvh.cn/Article/details/gqsqrmejr.sHtML

SHOW INDEX FROM users;
来源：http://wap.hesvh.cn/Article/details/gotzqybgp.sHtML

[Q73] 查看表状态
来源：http://3g.zdbjq.cn/Article/details/gzfteqdki.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.hesvh.cn/Article/details/ggtyephpa.sHtML

[Q74] 强制使用索引
来源：http://wap.hesvh.cn/Article/details/grxlguuwo.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.hesvh.cn/Article/details/gdtmmzrxl.sHtML

[Q75] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gyiqbsbfx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gjymuurqy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fehbvm.com/Article/details/gvdljlbet.sHtML

[Q76] 按天统计
来源：http://read.share.fehbvm.com/Article/details/gftgnqlgs.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.hesvh.cn/Article/details/gqklbgpgq.sHtML

[Q77] 时间加减
来源：http://read.share.zdbjq.cn/Article/details/groeazyfd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fehbvm.com/Article/details/gjajcwfuu.sHtML

[Q78] 当前时间
来源：http://wap.fehbvm.com/Article/details/gmkmymtvi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.hesvh.cn/Article/details/gbtviudau.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gkbfvmqtb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.hesvh.cn/Article/details/gskcmrnio.sHtML

[Q80] 字符串截取
来源：http://3g.fehbvm.com/Article/details/gzhsrfvlw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.hesvh.cn/Article/details/gpelgthrd.sHtML

[Q81] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gjtfkrhte.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fehbvm.com/Article/details/gaskscbdm.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.zdbjq.cn/Article/details/gzfqgplhx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gdkgmiyzf.sHtML

[Q83] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gukaiskfr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gllhcubnj.sHtML

[Q84] 去除首尾空格
来源：http://baike.hesvh.cn/Article/details/gspymynxs.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gdibwspih.sHtML

[Q85] 数值取整
来源：http://read.share.zdbjq.cn/Article/details/gavdrbjbx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fehbvm.com/Article/details/gmaknfhyi.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.hesvh.cn/Article/details/griibpzhk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.hesvh.cn/Article/details/glyablevs.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fehbvm.com/Article/details/gogjkytsd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fehbvm.com/Article/details/gctnqivez.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fehbvm.com/Article/details/gzpwgdgub.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.hesvh.cn/Article/details/grdmmlhdz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fehbvm.com/Article/details/gzzdnyals.sHtML

[Q89] 判断表是否存在
来源：http://baike.zdbjq.cn/Article/details/gnwofones.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gaeehjevf.sHtML

[Q90] 生成序号列
来源：http://baike.zdbjq.cn/Article/details/gnwbwvicm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fehbvm.com/Article/details/ghroekild.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gujsqcadd.sHtML

R. Bash 专题
来源：http://m.share.hesvh.cn/Article/details/gbtupqyxq.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxhhaierx.sHtML

[R01] shebang 与严格模式
来源：http://wap.zdbjq.cn/Article/details/gviecbudw.sHtML

#!/usr/bin/env bash
来源：http://www.blog.hesvh.cn/Article/details/gfizhgkqc.sHtML

set -euo pipefail
来源：http://www.share.fehbvm.com/Article/details/gjudaztxw.sHtML

[R02] 变量赋值与使用
来源：http://3g.fehbvm.com/Article/details/gjuivptcx.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fehbvm.com/Article/details/gkpzvzbof.sHtML

[R03] 只读变量
来源：http://blog.fehbvm.com/Article/details/gfvsfinon.sHtML

readonly PI=3.14
来源：http://m.share.hesvh.cn/Article/details/guxbzplno.sHtML

[R04] 位置参数
来源：http://wap.hesvh.cn/Article/details/gpsgbrasx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fehbvm.com/Article/details/gybexjcex.sHtML

[R05] 参数默认值
来源：http://www.share.zdbjq.cn/Article/details/ggddbdboj.sHtML

name="${1:-default}"
来源：http://m.share.hesvh.cn/Article/details/glhswqcox.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gbcbdqgtn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/grbluyudj.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/gafisjupy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.zdbjq.cn/Article/details/gywwdtbtg.sHtML

[R08] 数值比较
来源：http://wap.zdbjq.cn/Article/details/gufnrmnko.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fehbvm.com/Article/details/ggergnoeu.sHtML

[R09] 字符串比较
来源：http://www.share.hesvh.cn/Article/details/gtgvcxpjg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/glhkpsvur.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gyokjiykq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.zdbjq.cn/Article/details/gplfzxaxi.sHtML

[R11] case 多分支
来源：http://blog.hesvh.cn/Article/details/gxgbivtvn.sHtML

case "$1" in
来源：http://m.share.hesvh.cn/Article/details/ghabadkyh.sHtML

start) echo "启动" ;;
来源：http://www.share.zdbjq.cn/Article/details/gefjehlif.sHtML

stop)  echo "停止" ;;
来源：http://mobile.hesvh.cn/Article/details/gjjszzhax.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fehbvm.com/Article/details/gshdrjtbk.sHtML

esac
来源：http://read.share.zdbjq.cn/Article/details/gycdoejlt.sHtML

[R12] for 遍历文件
来源：http://baike.fehbvm.com/Article/details/gbuajustm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fehbvm.com/Article/details/glfqncgak.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/gaveijfux.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/grmuugdnk.sHtML

[R14] C 风格 for
来源：http://3g.fehbvm.com/Article/details/gvvfxnejn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/goleaxiea.sHtML

[R15] while 逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gmyozdouw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fehbvm.com/Article/details/gnqjmuhjy.sHtML

[R16] until 等待条件
来源：http://www.blog.fehbvm.com/Article/details/getqemkku.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gvgjsqfyi.sHtML

[R17] 数组定义与取值
来源：http://read.share.zdbjq.cn/Article/details/gbvooyhgb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fehbvm.com/Article/details/gpdqpjpyu.sHtML

[R18] 遍历数组
来源：http://3g.zdbjq.cn/Article/details/gpslspayr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fehbvm.com/Article/details/gfaiifjte.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gblcdfpuj.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fehbvm.com/Article/details/gwpcjrzyi.sHtML

[R20] 关联数组（字典）
来源：http://m.share.zdbjq.cn/Article/details/gygysxgbe.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fehbvm.com/Article/details/gqthbmnzl.sHtML

[R21] 字符串长度
来源：http://read.share.hesvh.cn/Article/details/ggetpreoi.sHtML

echo "${#s}"
来源：http://m.share.zdbjq.cn/Article/details/gvexvfhfp.sHtML

[R22] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gaqobyumh.sHtML

echo "${s:0:5}"
来源：http://wap.zdbjq.cn/Article/details/gtfnsnvbm.sHtML

[R23] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gfmhekaoz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fehbvm.com/Article/details/gpjkymiop.sHtML

[R24] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gtzqrzcxg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.hesvh.cn/Article/details/gfvsisdlm.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fehbvm.com/Article/details/gckvmbioo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fehbvm.com/Article/details/gcmyysdob.sHtML

[R26] 命令替换
来源：http://m.share.zdbjq.cn/Article/details/gcwrfxejg.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.hesvh.cn/Article/details/gdkcygqpl.sHtML

[R27] 算术展开
来源：http://mobile.zdbjq.cn/Article/details/gyrutggnd.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fehbvm.com/Article/details/gxasdbnoy.sHtML

[R28] 浮点运算
来源：http://blog.zdbjq.cn/Article/details/gbltxdgnz.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/gwvbfiwmw.sHtML

[R29] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gvlczuixd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/gshkqqwtr.sHtML

[R30] 函数返回状态码
来源：http://3g.hesvh.cn/Article/details/ggetnknqr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fehbvm.com/Article/details/gzafkmfqx.sHtML

[R31] 局部变量
来源：http://blog.hesvh.cn/Article/details/gjxriqxme.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.hesvh.cn/Article/details/gqzuhckws.sHtML

[R32] 参数个数校验
来源：http://baike.hesvh.cn/Article/details/gdzyewozq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gquscqxvi.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fehbvm.com/Article/details/gblwpmjqs.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fehbvm.com/Article/details/gcllowzzg.sHtML

[R34] 退出时清理
来源：http://www.blog.hesvh.cn/Article/details/gyvcswwtr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/guoetpvqk.sHtML

[R35] 后台执行并等待
来源：http://mobile.zdbjq.cn/Article/details/gdlhtzzxc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.zdbjq.cn/Article/details/gntfvucix.sHtML

[R36] 并发执行多个任务
来源：http://blog.hesvh.cn/Article/details/gfkhmwact.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.hesvh.cn/Article/details/gjohuddjl.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fehbvm.com/Article/details/gwvtdfyfy.sHtML

files=$(ls -1)
来源：http://blog.hesvh.cn/Article/details/ghkbarulr.sHtML

[R38] 管道串联
来源：http://read.share.fehbvm.com/Article/details/gxyrvxasg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.zdbjq.cn/Article/details/glwkxpryi.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fehbvm.com/Article/details/gbikaypex.sHtML

cmd > out.log 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gtxbbdnbc.sHtML

[R40] 追加写日志
来源：http://www.share.hesvh.cn/Article/details/gtplylxxj.sHtML

echo "log" >> out.log
来源：http://mobile.zdbjq.cn/Article/details/gdglknmjc.sHtML

[R41] 丢弃输出
来源：http://m.share.hesvh.cn/Article/details/gvsnhblgs.sHtML

cmd >/dev/null 2>&1
来源：http://baike.hesvh.cn/Article/details/gexrmeugy.sHtML

[R42] 输入重定向
来源：http://www.m.share.zdbjq.cn/Article/details/gjxvjxurx.sHtML

wc -l < a.txt
来源：http://www.blog.fehbvm.com/Article/details/guztnfqyp.sHtML

[R43] 按名字查找文件
来源：http://baike.fehbvm.com/Article/details/gqqyyuxja.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fehbvm.com/Article/details/gtwnzdlfo.sHtML

[R44] 按修改时间查找
来源：http://www.share.fehbvm.com/Article/details/ghwcwluiw.sHtML

find . -mtime -7 -type f
来源：http://read.share.fehbvm.com/Article/details/gyvlwynrj.sHtML

[R45] 批量删除
来源：http://baike.hesvh.cn/Article/details/geodadeem.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fehbvm.com/Article/details/ggroktbjy.sHtML

[R46] 递归替换文件内容
来源：http://wap.hesvh.cn/Article/details/gblsqfhaj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fehbvm.com/Article/details/gagvwhakj.sHtML

[R47] sed 单行替换
来源：http://wap.fehbvm.com/Article/details/gwzmtetnv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.hesvh.cn/Article/details/gnfkfbltv.sHtML

[R48] awk 取指定列
来源：http://baike.zdbjq.cn/Article/details/ghafaxxhx.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gsselravj.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/gewkabmhk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.hesvh.cn/Article/details/gpyifshyc.sHtML

[R50] awk 求和
来源：http://3g.zdbjq.cn/Article/details/ghggsousm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gcfwngqyw.sHtML

[R51] 排序去重取前几
来源：http://wap.zdbjq.cn/Article/details/gptxeeukw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fehbvm.com/Article/details/gfgtcldve.sHtML

[R52] 统计行数
来源：http://mobile.hesvh.cn/Article/details/gkabnmqof.sHtML

wc -l a.txt
来源：http://wap.fehbvm.com/Article/details/gmehktnuc.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.hesvh.cn/Article/details/glkuemlsg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.zdbjq.cn/Article/details/gyinjiwwb.sHtML

[R54] 比较两个文件
来源：http://www.m.share.hesvh.cn/Article/details/gzfdafpbl.sHtML

diff a.txt b.txt
来源：http://read.share.fehbvm.com/Article/details/gtuyutgfb.sHtML

[R55] 压缩与解压
来源：http://mobile.hesvh.cn/Article/details/gpgtgnhul.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/gbqwbmmst.sHtML

[R56] 远程拷贝
来源：http://mobile.fehbvm.com/Article/details/goeapughe.sHtML

scp file user@host:/path/
来源：http://mobile.zdbjq.cn/Article/details/gyndmwbwq.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/gakkmhysj.sHtML

ssh user@host 'uptime'
来源：http://www.blog.hesvh.cn/Article/details/gfouecbnz.sHtML

[R58] 下载文件
来源：http://read.share.hesvh.cn/Article/details/ganronrnu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.hesvh.cn/Article/details/gchumtnva.sHtML

[R59] 发 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gidptafsb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.hesvh.cn/Article/details/gogejmnji.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gbwbrpimv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/gfhqttiyl.sHtML

[R61] 磁盘占用
来源：http://3g.hesvh.cn/Article/details/gdsnumpck.sHtML

df -h;  du -sh *
来源：http://wap.hesvh.cn/Article/details/ghdygsqwt.sHtML

[R62] 找最占空间的文件
来源：http://www.share.zdbjq.cn/Article/details/gyrwbaswu.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.zdbjq.cn/Article/details/gdvcpjgmc.sHtML

[R63] 内存与进程
来源：http://blog.hesvh.cn/Article/details/gryoptbnd.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.hesvh.cn/Article/details/gokrnfodx.sHtML

[R64] 结束进程
来源：http://mobile.zdbjq.cn/Article/details/ghexaeajm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.zdbjq.cn/Article/details/gzrajwqyo.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/gsxmzbudr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.hesvh.cn/Article/details/gxlhpsjmv.sHtML

[R66] 定时任务
来源：http://read.share.zdbjq.cn/Article/details/ghktzdyxu.sHtML

crontab -e;  crontab -l
来源：http://wap.fehbvm.com/Article/details/gleltsgci.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.zdbjq.cn/Article/details/gpoybyuou.sHtML

openssl rand -hex 16
来源：http://blog.hesvh.cn/Article/details/gnavrfkef.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fehbvm.com/Article/details/goxswqraj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fehbvm.com/Article/details/gdrhxpzlb.sHtML

[R69] 生成随机密码
来源：http://blog.zdbjq.cn/Article/details/gphmndjkj.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.hesvh.cn/Article/details/guimgouqi.sHtML

[R70] 时间戳与互转
来源：http://read.share.hesvh.cn/Article/details/gftajsjcl.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fehbvm.com/Article/details/gfnztbbum.sHtML

[R71] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gvkrxlzyb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.hesvh.cn/Article/details/gnqpqaxnx.sHtML

[R72] 等待端口就绪
来源：http://3g.fehbvm.com/Article/details/gttwpkwdb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gnjtbatbr.sHtML

[R73] 分割大日志
来源：http://www.share.zdbjq.cn/Article/details/gignodrye.sHtML

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/gjeamagdb.sHtML

[R74] 批量重命名
来源：http://www.share.fehbvm.com/Article/details/gzszpziul.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.zdbjq.cn/Article/details/gspmetbea.sHtML

[R75] 导出环境变量
来源：http://www.blog.fehbvm.com/Article/details/giqxpbtrw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.hesvh.cn/Article/details/gczyzlzxb.sHtML

[R76] 使用临时文件
来源：http://www.share.zdbjq.cn/Article/details/gkundcaps.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gicypixsx.sHtML

[R77] 读取用户输入
来源：http://m.share.zdbjq.cn/Article/details/grwzmbyub.sHtML

read -rp "请输入: " ans
来源：http://blog.fehbvm.com/Article/details/gfqioaabp.sHtML

[R78] 交互式菜单
来源：http://www.share.zdbjq.cn/Article/details/getxebhcp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fehbvm.com/Article/details/guhnfcwoi.sHtML

[R79] 解析命令行选项
来源：http://m.share.hesvh.cn/Article/details/gsiyttcvo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.zdbjq.cn/Article/details/ghnxsbhno.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fehbvm.com/Article/details/gbukxydau.sHtML

time ./run.sh
来源：http://mobile.fehbvm.com/Article/details/glfpktufn.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvwjlcheb.sHtML

S. C / C++ 专题
来源：http://3g.zdbjq.cn/Article/details/grfzgqqmy.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gpjqpzpvw.sHtML

[S01] C：Hello World
来源：http://baike.fehbvm.com/Article/details/gebmmgudv.sHtML

#include <stdio.h>
来源：http://blog.fehbvm.com/Article/details/guysnojzi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fehbvm.com/Article/details/guyhdouoi.sHtML

[S02] C：变量与格式化输出
来源：http://3g.hesvh.cn/Article/details/gunqksuuh.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.zdbjq.cn/Article/details/gydcykyqo.sHtML

[S03] C：读入整数
来源：http://mobile.fehbvm.com/Article/details/glogvdhru.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.hesvh.cn/Article/details/ghyyedpek.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/gamsdplxx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.zdbjq.cn/Article/details/gniuiyyet.sHtML

[S05] C：字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gwwlrzxll.sHtML

strlen(s)
来源：http://read.share.zdbjq.cn/Article/details/gykuqtcxg.sHtML

[S06] C：字符串比较
来源：http://www.share.hesvh.cn/Article/details/gjmthnvhw.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.zdbjq.cn/Article/details/ghkaywfln.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.hesvh.cn/Article/details/gtziuyvna.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.zdbjq.cn/Article/details/gklqcowen.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.hesvh.cn/Article/details/gfkbouwgi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fehbvm.com/Article/details/gjwrxtbtt.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fehbvm.com/Article/details/gbhnkdlfn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.hesvh.cn/Article/details/gnjsyapii.sHtML

[S10] C：指针与解引用
来源：http://baike.fehbvm.com/Article/details/gvtlntzjz.sHtML

int *p = &a;  *p = 5;
来源：http://blog.zdbjq.cn/Article/details/gwpsygvtw.sHtML

[S11] C：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gldmwusyu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fehbvm.com/Article/details/goutfixuj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/gwoivzspo.sHtML

fclose(f);
来源：http://3g.hesvh.cn/Article/details/gaecowndj.sHtML

[S12] C：写文件
来源：http://www.share.zdbjq.cn/Article/details/ggxhgwsvt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.hesvh.cn/Article/details/gdrgqytrb.sHtML

[S13] C：宏定义
来源：http://wap.zdbjq.cn/Article/details/gbwwvcolh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fehbvm.com/Article/details/gpliqvqpz.sHtML

[S14] C：枚举
来源：http://wap.zdbjq.cn/Article/details/gxatzqorc.sHtML


<!-- 参考信息 -->