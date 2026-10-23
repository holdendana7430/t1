代发 wailian999

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3kxugbczt.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3vmjcqxej.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3jihoynoq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3geektoyh.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3dbilqtph.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3irfpbcei.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3knsuqmre.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3qarohdbf.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3pximxgre.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3phopbllt.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3gpwvgdar.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3fzrkkapj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3xqkvduay.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3gpvicpzh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3mcmbxwnp.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3ztcbjcqm.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3bvoejgjc.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3txsuzajk.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ktftvlfq.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3pfvblcdy.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3toeydpnj.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3paonvsfe.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3ggntuevb.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3usrxqono.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3uvssayia.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3qqjmmrmg.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3vxnvhqyg.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3yhbgfxmd.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3syhbobnc.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3bdgayedj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3djjugtuh.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3tbcvncbn.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xntbbcof.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3jfquvlzo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3ypkqpoow.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qdbvseue.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3esjqgkbl.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pjmmxkng.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3stysxdop.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3vidylnwo.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3sxjqwzjp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3uveaxfbl.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3tkxwotzp.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3qldaskoi.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3pgluvzhz.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3vxcpvtuq.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3ogmasrtu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3kcldbxke.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3tcnwklhg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3aiauysno.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3xhcncomz.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3orhrcwho.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3irfkllpc.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3zubhvqfe.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3ebiybesv.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3zpiqtykn.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3pxpmdmph.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3krnhzalt.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3dhzezsny.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3eqsfriqj.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wktblvfj.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3vuhewmed.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3hlrlvogy.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3mperarqz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3abyifxzi.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ffbtvgvs.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3lbvytqhf.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3bylorhlq.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3vxprbxbp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3ijbsudli.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3hnveduxz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3vyihlqcv.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3xdqtizde.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3uoduebwu.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3tpzhfnii.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3dnkfrhgu.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3ogdchory.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kmabhhgf.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3pypcnezt.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3frqbzmha.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3czcyhoxk.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hwqyjxrv.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3pvdqevip.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uvkmbztj.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3hhtqkqpl.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ubodsfxa.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3ydstuuto.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3rfrwilpf.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3hmujvaew.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3xklzvpmr.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3lbawkzmt.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3dhqklocp.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3afwhguid.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3txdyxihr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fvpxttjk.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3gmxlzyvp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3yfkboxxr.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3dcncyakj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3owfgyleu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3duvwzeue.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3irxzrsen.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bojarwsi.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3bmhlzeuq.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3cyltofni.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3gtbeothu.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3mshwpojd.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3vxnwjmyw.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3ntwulcnj.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3eevholqg.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3coittknc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3htjwykqr.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ynmisaeu.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3tbclkdmb.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3eucycixe.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3lnwtfwsd.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3tzrtezrt.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3dxvfcrvo.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3zdunqveh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3gvrswlvl.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ziugmljd.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3cckgmwkg.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hwucsqpn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3zaqzsnpz.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3niyjyios.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3achwmelw.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3einguvyu.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3ykcxvcnb.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3xblynzoi.html

esac
来源：http://www.52xcode.cn/Article/details/gt3hlsvmewq.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3zupgahyb.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3ufyyrmrv.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3fucperqf.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fnnnfchu.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3tcwdcnvu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3qfubznra.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3deimodqo.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hyonjhmh.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3njdzmnvm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3xpnvukok.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3dfjutnzu.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ydfsnmqx.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3ljdtoiav.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wncuuqvm.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ppspcbta.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3ipzbzsoe.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3dctuvbas.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3bragqfay.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3xgduqbpo.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3svfbgpqu.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3nbysklpf.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3upzjhtmk.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3fhdwrogv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3xxnntnjl.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3iyvyhqqt.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3dcqtbrot.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3vznyvppa.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3dowgcjti.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3yhgtldil.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3ohdofjhy.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3hlsuraxe.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3kiwwvkkp.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3aahfsvlo.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3yjthcszx.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3lksccyjd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3ozbgtfwi.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3gyoflcop.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3hfaislku.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3jcmhqdjl.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3fvyufpzl.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3dozhkcvg.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3otyjikro.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3wnanpmey.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3vdoeieyn.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3mnznwfrw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3lkrewsgt.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3sdetqbyb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3prpjftzi.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3rgfqfmfj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3vomogxfb.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3gkdczlqq.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3zrigvucd.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3kogsgtld.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3buoezbhv.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3uqyubkef.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3moqyhbif.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3xdyxzdkp.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3waziglzm.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3oqvqgxnx.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3fuymasas.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3dvevjpjk.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3wpzltidf.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3upghiryc.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3fiztddbp.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3hbztikjc.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3shwldxna.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3anvmkksv.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3apnlsdxe.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3lyxnfktb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3ojlvacfh.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3yuaacldn.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3aslhhutk.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3odxtvrlu.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3annfdtnv.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3givnqmhl.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3rlobkure.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3kwdidjbr.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3afwopsdh.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3iyiavyxb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3zfdceqyy.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3agfrcmvn.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3cxsprzoe.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3zqgbigxp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3spsjhpvb.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3podxkjqb.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ajvmziym.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3ilgvpykx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3ipdvvmpv.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3nkaubtci.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3oiekbrro.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3yeljiggo.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3tudjntvf.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3eivmpcly.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3cnsxhbnx.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3qjkslghx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3szosenwi.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ocyzynxw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3nbhjasix.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3omwigeur.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3lwxilscy.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3urzgmnty.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3sjpcwcki.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3polsjafs.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3iodwoflh.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3ehntzfla.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3gnxhkuuw.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3djcmzvxo.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3bincoqcs.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3wdhjvdjh.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3dlcgeumi.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3ogagglmo.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3exptgpje.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3ylkglzxk.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3zuncihfi.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3owsyljbm.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3spsqqbch.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3bizxcbxt.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3fnktyvwj.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3mioawird.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3idpadajq.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3ildqvtdo.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3spxraxvi.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3fdkbikkj.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3itafapxe.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3upajdkaq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3myjxmsry.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3aiiofoss.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3ttkkjaaq.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3yqpwndxk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3wtwiibze.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3qotqadzo.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3kiileqri.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3rggsdijl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3wrhqxttk.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3gdkbweyt.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3wzvtgwno.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3xlokmohg.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3lgzcthem.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jcpomzis.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3uxxwvsgw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nagqwfjt.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3iusuzxjw.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3upygpmbz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3glzrlkii.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3ndewdmln.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3atyxvrdj.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3uzlohcfo.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3uplavfnn.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3hftlptzg.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3osumjekk.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3avmusujt.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3twuaqfms.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ubtepkfn.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3jwsuodla.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3cvvqmhip.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3ywngbmfg.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3lcauwjcf.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3jenqbges.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3nnqxrghi.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3uiahokyo.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3ohenpkqm.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3utctyuzg.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3rvpdvufw.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3bepzvdps.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3bqzuqhwf.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3lxuqvygd.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3zbifyzrq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3hpeitnus.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3lwelwetc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3asghfeue.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3qskqympf.html


<!-- 参考信息 -->