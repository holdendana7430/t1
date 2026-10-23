代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3wbylkstx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3krnkukrf.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3evvaidwx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3wurwuybm.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3rqiuzaga.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3fvzwnekq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3jebnpzmm.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3jdrhcyeb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3rrnmriiz.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3jebotiak.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3kpamftzy.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3kixwowgm.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3axwxohdm.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3tifaxidg.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ugxgledr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3ecnrmbam.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3zzdzloxi.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3rikcyfxr.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3ixjewhyw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3dqcqxljz.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3fugbzprb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3qaddwakf.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3iwxcoimv.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3xwpattcr.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3jdaeinos.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3nephjxqg.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3idthhxde.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3szwqqqlc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3hhypflro.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3uzrvdkmq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3tlzeuass.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3mqcxgjey.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3exlucnnr.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3rbqyoevs.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3qenpjmxh.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3akynzwud.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3hompmoem.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3qnvcubes.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3ewjwtqxx.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3tjhycuul.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3tccmpppo.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3erojxbfs.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3jkcxwutf.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3eesnajfz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hisliagb.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3gjdivxqe.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lxbkkqsz.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3wjqtvimg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zksssyya.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3akrqjdrr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3fknxcrlk.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wmizaout.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3semyeith.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pbtqtevc.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3sarlgxav.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3okfboyup.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3kqxlefky.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3sudkkojb.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3zuuzgxyb.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3lujojtwq.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3chssvpjd.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3azjtpcph.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3ukcbmorj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3xjwmtyzu.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3ybbihoct.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3zlusfugh.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3wsgwpcgd.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3iqkmlovg.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3bsohiuen.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3uczcewwl.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3rinkoeio.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3reygnfag.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3vgauwbzl.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3dvrhlncz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3rasdxwdw.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3odnbbfby.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3awoezmht.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3nuhmuhvg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ynjumzql.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3gfcwxzqx.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3njlxuwss.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3cpceelru.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3urfvoory.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3wyvdydtn.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3ikcvherl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3zmsvvkbr.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3gkrllocs.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3lwkdmfjq.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3jswsvgzj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3xgmggwgn.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3swkwjvtx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3gxrvzdng.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3dxtpepwb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bdyvazts.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3mcxqflsz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jxlzcmre.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3mheegctc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qynzdxww.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ntiodavi.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3omyimswb.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3mgujxjnm.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jmbzfdwp.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3ajgrybfs.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3venyxwdy.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3auvhqaph.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3hjclxsvs.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3bulkeoke.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3lbdattjv.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3wkiqlxjn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3hxjfdepc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lmktxpev.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3munrxbsb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3lkaygebe.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3emsqeeit.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3bcghmdak.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wrxevmra.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3onrerodd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mtbdhbcs.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3teyjghop.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3mhlwzmeg.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3bcfuaekg.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3evzfznuw.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3xgoywsfb.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3pumuyhmn.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3xxqvpkos.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3ixebijea.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3pucpsqcw.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3mldrbvln.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3qirkvbkr.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3dawcbazk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3fcnacjnz.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3mtwzxkzt.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3fydwvgnu.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3fydvqrbx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3rdwbchty.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3pbfodgfh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3zqrlvjmf.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3ldhshgss.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3sabehmkk.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3kibptceb.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3dqxqusbw.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3oziwpxcd.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3fxfwaxpm.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3pvorfvvy.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3ordpruyk.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3kduztroy.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3dmgyepuf.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3wuuqhxyk.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3tyaoimze.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3qtupqdtb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3icrhbzoz.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3tphlyfvh.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qqsdjtue.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3kqgcoljk.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3dqhhpgxw.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3jwaoisch.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3wxcjurgy.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3vmodhrhu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3wsaaqmgz.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ijudyyjw.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3mqwyigrf.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3gvgmpmgb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3bsuxxcbr.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3fspuncfs.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3nvzrgvod.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3cjzvtqgm.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3ztvlzhjk.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3gyzegrxm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3eroxisui.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3qihvtbor.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3vlxhqput.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3mvzjnrhk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3uawcgfed.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3hafxhdah.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3pmgmtqhu.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3fzgdleen.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3nqsfseuq.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3sxwufsul.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3loycuxvr.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3dtubpujo.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3zglfjzvj.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3jolbvxor.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3gckefcyd.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3dsoflqpi.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3cbvgwiae.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3rbfydzkb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3wauijtqy.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3jyivmbbg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3vdwjwsqe.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3zjcjykxf.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3ruepitpx.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3ulllnimb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3iznkfnau.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3oxhnjacu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3ipydyksq.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3qpotmkoe.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3knyhhxqz.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3omiyvkzj.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3dkfyzylb.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3tbgliplu.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3jverhzfn.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3zfgschoq.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3hdrwutzc.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3vlecrsdy.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3kvfenrtn.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3xohxktzf.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3jxyswcvz.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3qvaongrz.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3tjowapzt.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3lalgihkr.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3kysbcqkx.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3wsuvpnag.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3ukvdwznw.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3eoxqagaf.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3wsgigroy.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3qsmynefi.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3luahakkj.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3qmklwxgt.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3xumuuxsm.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3torxfaan.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3pmocizrf.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3efezqtkh.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qzhgovof.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3pgiydsbs.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3cewwneup.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3fuybxrkp.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3yizqjbtx.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3puqjlsmt.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3fptortkb.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3hjoshxel.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3poxnntok.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3nzvziryq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3iwivyuzl.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3nvkyffch.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3whbgnoqx.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3eouwaatx.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3csricxcy.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3uvrpvapg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3rwcxkeki.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ajmvxxjl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3aiacsbsg.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3wcstxkcx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3xymoqjxr.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3fwyyawlu.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3wnonntpy.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3arfhwzrz.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3nruzydow.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3wiopixfl.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3xboanbuo.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3ptcqgbqz.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3qudnjqfj.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3yiiklgnh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3xbepggcy.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3fjqmywwt.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3fzgblvvz.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3qoqxmaao.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3enjszmeg.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3naxynlpg.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3rutvnejj.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3cgartbff.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3ycdpwvlu.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3oalqmsjm.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3oiktxazp.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3pxeylbkw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3gsfacpxr.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3demxsjzn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3hmbvjsje.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3shttnbeh.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3zzkrsopk.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3ikkrgivt.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3lxufoovr.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3hckgwpie.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3lkljpxod.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3mftgmfkr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3otuegukd.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3bsqtrzij.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3yeodshxm.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3rtecmvvh.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3bqynddvy.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3kvyganfd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3baxhqwgh.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3pcmnkciq.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3hybllwap.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cabvzpwk.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3sbedrrqy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kmrckpji.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dqbqdbrn.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3zztiefte.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3phfpnqpk.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3ecieqequ.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3vaiwuten.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3pgefxrsi.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3zltgzpfn.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3ojyngwen.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3gnxcewuh.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3jpblbdqp.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3mnmwlvzf.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3nojluedw.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3idtbsodb.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3bsdbajyy.html


<!-- 参考信息 -->