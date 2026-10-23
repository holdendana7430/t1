代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3ityqrjtm.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3xjitwpzg.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3nuqpcdju.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3hgxdmwhn.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3dtfjmxqk.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3foavsixg.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3xtqipych.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3evrqtrge.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3npkvdxar.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3fndfmapw.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3zlshorwv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3lqbwykvj.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3buicxupo.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3tsqklsph.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3dzdctrei.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3rojljynd.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3mtcmxbvt.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3emklxxku.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3matblhjs.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3dihmoqye.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3jdipmtqq.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3uegnfgzt.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ueojtcyu.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3fctjnirf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ajleazvg.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3lihkzofo.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3isxoxeti.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3npbjcbhy.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3rzvzghdw.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3xtsodpnl.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3yhtozbea.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3xbeqrsyj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3wllxdnbh.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3vsposrpj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3dmxxmprd.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3wtsghmdi.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zsdzlhrz.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3sgpakcbh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ffwdfabj.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3qvgwdumi.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vfmovbpq.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3dnojgwko.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3nunuxlwn.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rfamokuj.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3wbhydofy.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gqukctod.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3itpucbvu.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3qaggzkbe.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3qcqjzyop.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3asdonekh.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3vsytawha.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3chahffpp.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3lbjbongp.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3vfdfkxsj.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3uwqaoqlb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3bcpwzzmh.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3zjnrwrwd.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3kycaownh.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3aogvksqn.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3pxtsvxcj.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3wjuoidtq.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3yqzuuxix.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3nlapvssb.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3loeywtcr.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3hocgqdxc.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3bxtdcrfn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3ztgmlncd.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3bfspictq.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ezhtbftr.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3isffjizo.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3eoarnjom.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3dezlpcgp.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3mathsmwn.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3kqmpftao.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kjvqwsaq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3dfzymgev.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3hhcdkplg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3xlcupcvb.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3mdkoncqh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3baehfewf.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3ebeodqdh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3jdvygiqb.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3kxfzlxeo.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3evhtysuq.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3jxlpnzit.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kprgngzr.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ibytzlwe.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xjycohiu.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3ppvpiwsb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mirtpszx.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3zskipuuk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xegexclv.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3eoyasavn.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jgkcfent.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3hwavzjuf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3vytceban.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3habaffli.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3vfwixlqb.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3qsccyeoa.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3hgzvoxhh.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3stayvblb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3ipdjvygr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dnufwjll.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3lntxquly.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3ilgvhltf.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3ydxoahkd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3leflekuj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oejxmumr.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3yiflcnmq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xjhyhlok.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3ncnyxmax.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3iccchwdy.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3uuwstrrb.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3qmpnvbpr.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3bqrgvpfe.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3adgsegne.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3hwunfzzq.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3ppgoylok.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3dfengbqh.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ymcckuni.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3rogubbfe.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3jrdfxcaw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ujfgfhel.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3dztxzuwf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3uhgtfxta.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3jxrpqiwq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3psrvewmp.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ypcrgixc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3vkkhbcts.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3nzkioxog.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3gjqzdenp.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3vvrltluh.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3omgfklvt.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3avwqwapq.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3iibgfejy.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3acrvhkei.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3ouxjvttc.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3ibjvybiy.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ouavelkq.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3dtbsknyo.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jctvympi.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3adshgbac.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jtqwxnqs.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3fwylypys.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3umhbdsfr.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3ptddszqr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3tzitakqy.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3qzdeqpnu.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3sporefwh.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3gaunnczv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3rlbznnzp.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3rtktlrag.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3waezsmad.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3sweqmsem.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3inswkknu.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3drcuapkj.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3ezhbmlns.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3xgwooqxq.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3brtuzwia.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3skbrkpev.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3qajgfhie.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3fbpvfpqs.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3lhkyrjqp.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3yficcdoj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3pikuhuvt.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3lnhrkuyn.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3vcvhfkyt.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3bsvazfks.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3fsfzyjsm.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3ffwzvtfu.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3rdtgnfwy.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3mootvrjz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3yderpdlg.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3jjrgvjgi.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3zqhfzfsb.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3nxofstjd.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3obkjpuca.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3lmeqgmta.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3xogmumba.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3eqeluqig.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3ijncfers.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3sgsxzyge.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3xajoezqs.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3wjzosyih.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3zqzlulgb.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3qasvcmwa.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3itpoento.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3uaynjbxz.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3airobwom.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3wyzbgulp.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3dnwrdovm.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3yzbbfgju.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3diobvqfc.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3etjyfifc.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3dqritqrj.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3zkdrtgpd.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3sbhomuyp.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3ytdbseqp.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mdgamreg.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3dbhldksh.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3nkacstwj.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3eslcjztr.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3btkzqwuq.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3cfhhzcrq.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3zoejpges.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3vhhpmndy.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3crnimjsu.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3cgfcozpi.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3aszrxqon.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3hdtcolba.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3edyuehoo.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3seytfkdb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3fmxkgurg.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3kbtyhglo.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3imynekwi.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3ijlsanqm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3tkpajrlk.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3tfvckroh.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3jxomamhs.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3yzfkscuc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3kwdclngm.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3sfixjhwp.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3wnaftsdr.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3vppjtggm.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3tnecbuni.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3rlneuarm.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3nhadfolm.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3jpfrxuak.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3hbtebtke.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3xfnszccq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3vcrsrykx.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3cxinqhjh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3fdmngikb.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3vdeqohlw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3gexelmvz.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3gjdjfmdh.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3pbdggdkd.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3kedmysse.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3yzuhzyha.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3ziebgxjw.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3gnzepjmj.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3oxsdgdxq.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3ffvqyayf.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3rgarbejy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3psmvcvzc.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3ulcglobi.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3jftasiti.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3jmtptotv.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3qpnzqrry.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3srgyuwoe.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gifosonz.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3iwlmrezk.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3ncgoipfp.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3zfyoetvg.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3fkrfuxwy.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3helbkqap.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3frwixomi.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3vbwyyhbe.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3zfhtmdml.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3cbdypcza.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3mwwotoxw.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3lwaaaqbd.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3jcfqggso.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3xegkmctx.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3wkszidkh.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3pvwuvaxt.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3epbbosor.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3wkxsyjnu.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3ycrusfqm.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3psppqlwk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3eihyzaxj.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3gpwsybgp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3jofkvnvd.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3zmbbuktf.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3qhpfxgha.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uttilrtv.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3ixwwjmwk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3juntzhie.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ofghqcmp.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3uxiaqdzu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3vkfyxdsd.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3vqolylpa.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3shieghja.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3odwxowem.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3exbrkhvt.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3duonuvmy.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3xcekfdvp.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3dypbdgfl.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3qlievkih.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3qigaytci.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3uujmfpvj.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3nmzzycki.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3rdadcuob.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3gqsrcnum.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3wcqdtgtv.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3jnpqqqba.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3anxrqvbi.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3dtqicnid.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3edrjwbpx.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3hgtspplo.html


<!-- 参考信息 -->