代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3wfhbftdr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3yklownuw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3hlvhckno.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3yopizsih.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3hrwmrhui.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3awudmldc.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3lcghsjcx.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3jdhnypci.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3gfuegltt.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ngalqrhz.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3rmahrzre.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3xnrwzzva.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3sysznrbk.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3akylhglw.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3gevbwpto.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3sbyppqlh.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3flieogbb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3hzgjraky.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3lfcggajr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3vuazjqqp.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3cgfqfjfb.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3ccryqqam.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3wypovsdz.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3grykbcxi.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3tanghqcx.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3nnecoqly.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3yiyxwnju.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3fqmzaprk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3spxbxcgg.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3zdfrkxxs.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3czibnjbd.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3hedvbeyu.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3dfkifdqo.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3ulxsaldo.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3mozggcbn.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3wjwzsvfw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3hijjtepi.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3hxlzbaaz.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3vzdkjztf.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3hfkrifyy.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bmfgkqqv.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3qnrdebuy.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3hjpvuxfr.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3drauyjqz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3yzrmnpic.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3hzqoosoc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3tromjwim.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3smrtthjf.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3fstncmap.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3auhnwudl.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3xbnywhqa.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3rwdaqflg.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3nxokisuc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3hfeejxor.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3mnuvtklw.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3sgfaokig.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3myyegbuu.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3lzooofpv.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3mavbjuzt.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3vwnmhqnf.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3qgbyppua.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3odvbvofd.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3hccllcfv.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3igfdicdl.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3pybyfjva.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3ngzxfpjt.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3lxqcgghe.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3pnwkgisr.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3jrnthlly.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3dsypaukz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3pnsnmvlp.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3akmhbbvd.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xlmrisfg.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3woheaphe.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ukkywifh.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3citjbtqh.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3wmathglk.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jmzzbyfg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3rcmlnvti.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3mhhikmoo.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3xbwiombd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3zqwavbpx.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3ctlvswtn.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3ibelrzjm.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3aamfhjnt.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3hoauzakd.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3cmtuacil.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3ljlrbcjq.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3ogxdzfjj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sfojwvnv.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3iphnvupj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vrkizawq.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3uzoxwjcj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zjprrkpt.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3rnudpbbc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qcqxvewi.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3uuxtbnhg.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ctpqbrno.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3wwwtgonr.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3sjfrawhd.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3yoaxpone.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3uwrovsve.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3apvjxsef.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3iiniizgg.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3zlnfpgkl.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3hgwizjwp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3npwboihp.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3ikvlsvgz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3qdpfmlhp.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3ggnshvwb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3iuvmemzl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mdqvhlcg.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3inpqbamr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uaghxcox.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3gbarfaej.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3kapnykml.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3bbacluzf.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3aufjqamu.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3chmghoyw.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3dooahige.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3agatnvni.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3puysghyb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3ogkgocwq.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3ywolgmem.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3zmnhublh.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3zcxgubmp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3wqrcmcac.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3drynepbg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3cdyyrtke.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ctpfbssq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3tjcponnc.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3amuyjsgw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3lnramdrq.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mwpqaqqz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3vnsbswpw.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3vrazphlj.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3oyautgkk.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3qnpvansj.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3nynbakgn.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3bdevxqbd.html

esac
来源：http://www.52xcode.cn/Article/details/gt3igzzscsh.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3wyzpsyrd.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3uyrgkygr.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ozplvkfl.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ndvfxocq.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3xyiabcvg.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3suzojhis.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3iljlnfes.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3uamxxqtb.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3bncvzual.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3oelbvdvo.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3orvmuvum.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3monbhwiw.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3ckjlsoug.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3cpswcyfe.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3gtdwyvhv.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ksdkwlho.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3sdmufxjf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3anwrqbat.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ojavzbyv.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3cdulgjmm.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3nvqcoqhs.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3wyceidfw.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3oiqmwjhm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3ayrloolm.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3voqoxbia.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3rrmghqck.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3syohcikz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3dqboaerp.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3afenmbtp.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3ieclnavq.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3msnfcyci.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3wzjufbiu.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3kzciojcv.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3zhgcqgqk.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ifbmytll.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3nlpixhuc.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3oiqmydvo.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3lvblgmjy.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3atrgxjnd.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3imoorsgt.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3opyuqlfs.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ikaolddy.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3qgfdjfkv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3lbsktbnj.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3vopqpapa.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3imxxlxqs.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3hkveqksm.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3phhguaiu.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3cspqvwgj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3wpyhcmly.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3ypgyywuy.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ptpfcypw.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3zxyeqvyx.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3ugxgylku.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3xwhvfhth.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3sfrheatg.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3lqthalil.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3dzocawnd.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3xblcyiwy.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3yhfvtnek.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3uunesnqk.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jsaqmmgn.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3vrenwbys.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3lyvslgva.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3eccoemxr.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3uzizowuj.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3vajctztb.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3uncnmmfh.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3rbbppckv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3umxigpyi.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3zomwecak.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xgcwbuvc.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3mupmyptr.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3gomrjkzr.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3avbeijcx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3udvqlzub.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3rtepsvct.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3seqvwgkl.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3zwppbtrv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3qdjuhovn.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3iuisexsy.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yymhlqzb.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3oejebhms.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3ynemzcfc.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3bihvjhao.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3vqfpdgqw.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3zkziyrhm.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3aljalvze.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3pqcprhze.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3psslbraz.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3naukthwh.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3yivbvfyn.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3kpccdznr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3golzspam.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3wkpsikqc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3rckbtkez.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3igbsqscr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3xgfedlcj.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3hdmltpdj.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3eupirczq.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3gbxpypyr.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3vnfjsdqh.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3foabymad.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3kiyrdmok.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3bhtznxgf.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3fgubmpbh.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3tdsozsef.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3hnglbxuy.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3blzqdmbl.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3dsnmpazl.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3gzgwpqfo.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3fgtjlysp.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3ldguhcng.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3oqtgchhf.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3lgxdwaqh.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3aodbssbs.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3ugxcxjvc.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3cxuxywqh.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3jitrhals.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3bjhaaoor.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3zcokuyis.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3vxzitqkv.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3towsftcg.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3ltikgkoo.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3menfdizc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3zkfylawc.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3uscjlfiw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3rivfvnaa.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3aacheeqb.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ovsmschf.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3mbboyayy.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3puaxknam.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3mzeqtroh.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3nawjcgds.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3qpopinqs.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3jmhmqhgm.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3nsnguxpp.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3luzckesz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ymqdukqj.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3kapwivdq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3amoowdjf.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hmtpoipq.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3fniaelen.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3zlcqofqd.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3gncmwcsr.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3sreunwmb.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3qrfqhwmc.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3gobizekz.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3chamctuo.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3agoiiykw.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3msixgftw.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vtvvekdo.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3lrlsefpp.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3krezwkqn.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3owbluqye.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3fitowcfx.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3vxeqtuzn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3mxaicotc.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3egoglmsi.html


<!-- 参考信息 -->