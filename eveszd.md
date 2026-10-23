代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3dmbuaziw.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3vfuiyxvw.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3waqoovuf.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3qnxcbsxm.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3zvpqfzjb.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3aktfymti.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ylbefomr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3lnbjljwv.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ajumjzcp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3hqrizeke.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3cxrzynno.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3uzubjbxl.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3zmutieox.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3bizouwhp.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3jcqmcthg.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3xzxbfjko.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3vlalntzu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3jtwakmxv.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3jalhdejx.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3tyoyjrfb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3lpjpxbjd.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3piioayia.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3xzwuncqk.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3qewcqebn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3cfdeiory.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3uhcfjgct.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3picqqbye.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3qbhfhybu.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3vwsoolhr.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3npckhapi.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3plqbhxxw.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3izzkgmxv.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3ziuoflrm.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3akjpzrgr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3tlmojepx.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3ionchsxt.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3divjluyv.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3xexuwiwl.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qumxtfqa.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3ofcfeqrq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gqikuabk.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3odnlodya.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3bduzsrlm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ljvnkhde.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3sdtgxqde.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wfmxhafz.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3nfuzjone.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3tftqyigw.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3lgsmdyea.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3olzaobhe.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3clwgfbvm.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3uawmspez.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3sflmnpgs.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3igxzzqba.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3bzxifiub.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3rqqmrmrt.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3jzuxchpj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3yzovgwpp.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3arlskyit.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3httzlocp.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3eapjxatc.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3nnlyabqe.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3updmkmul.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3ftjvsirf.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3sfwsptjw.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3bjnwewak.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3yukmzeqi.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3hhkdnlus.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3itkhraxl.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3xlhzbbtr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3cqihvkda.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3wmgyjnfd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3hdjaclii.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ihtfsnzt.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3rzakflpd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3qihlgabm.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3fatkmzze.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3dpilfswd.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3itrabdgr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3mwgnmegc.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3jfvzjzux.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3itsxtlan.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3pouadggz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3zdzpiugx.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3vgkhegtt.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ktxcujvp.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3cqhcixlg.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mvjvthgj.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3ebpwkiqe.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hlxizjpy.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3gtcrjxtq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ryzffjfj.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3ptunflgk.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rnwmlokj.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3pgpokpqs.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3liqoibng.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3okeyygyc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3lgnzzfjd.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3elrbwrjy.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3nhjqiqck.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3wpevoohj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3kazgwfvz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lkyecvdj.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3ywrdortr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3afsscgdg.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3yjovnyrn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3adczziim.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xijcnrui.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3wvigocvh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eonulsnf.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3tpghmunz.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3tecwmbac.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3azjiyjor.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3oxeqigcy.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3qtvcrwpc.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3kvlcslwp.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3elfskauw.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3wvxbvlcj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3ntcvgnim.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3nxlvplxm.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3izazrwzi.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3ecxzykuz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3fvfukqbw.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3htanjgsi.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3jdrcpzmy.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ubtlyjjn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ljsunbaq.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3vlwxighl.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3ezpxuhij.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pwxtnlwu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3cwlbpaws.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3odiwkosr.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3dzooucbh.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3cbvcrlny.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3oknkxpzu.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3qourlsow.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3etyutihf.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3wkzytpch.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3gvvufoxm.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3lojqqvdt.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3unrezmgu.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3sjpvqlci.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3vjvrftww.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3nvdcmiyz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3liwwttmr.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3jyefcgis.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3hoezeotx.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3clhaghxv.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3vhqqgzzq.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3vcpsscmf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3ewbaaheh.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3xzcftpzp.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3svngkbwv.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3gjhpambk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3asjjqdzg.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3vioqtftl.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3kksslyrl.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3wwwfewqq.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3adehnnda.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3tizjtzpz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3azvitoxk.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3zivvgpqy.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3tvwqdipd.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3wejhzgxy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3kjpofiuz.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3mlprcson.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3vrsuvwra.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3qgkexyvt.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3uvszianp.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3cygbhdtm.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3kxrlwzrc.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ruvyzxwm.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3gsjrnydm.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3vwsictnb.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3dzeytrtc.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3qdvwgltx.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3pcpzgqyy.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3mmibryep.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3pnwbtemf.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3bqqkcehk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3tlplqyvi.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3pgxmxnom.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3myholxhz.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3wxoaxsho.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3oqwehdtz.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3ajasviyj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3fkfgeyww.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3zawvkres.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3yxenacgk.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3fbmvrjip.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3ipetiwof.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3cyllmvff.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3axvyhhpc.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3sthesgpi.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3ximssjfn.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3geonbwnf.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3mdsbcftq.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3toidvddi.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hiyvoizh.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3ijhnfdlv.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3wqcvblzz.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3utgcnejn.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3cuhnhykw.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3jjcgswvg.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3uvgwkawq.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3qhfzfewx.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3hvpmgags.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3vhtucmcg.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mcncajxl.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3blktarhf.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lgqwxmgw.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3wwgeuvjh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3mvpewmnj.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3qwmjzbkx.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yhxallci.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3plwlppjj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3yvatuadn.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3agnzhsbx.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3wrbpkjor.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3tmwmzgvi.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3wlrzsodz.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3djwvzfse.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ipljxvcd.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3nkbyqkpf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3anpjxhbh.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3jqqgxgka.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3rrlelrfy.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3cdzsyznb.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3nioxtdvp.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3bsgzaabd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3keqxrknk.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ylxfxkvw.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3znaxpnfg.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3mlyopvhv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3gobvchhw.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3qvisbvhf.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3fffbmfzs.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3tyhhionn.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3ounhtszm.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3uvfqunpp.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3tazcltdk.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3iyojbsdr.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3ofxkxgno.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3btwhymms.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3hrktswdn.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3tjuamxex.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3dnleesfq.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3ybltpbzu.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3ittbimto.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3vaezkaxb.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3yhaosagy.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3xokodlnr.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3zpzxhzxm.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3myxmxcns.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3oynvazcr.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3usvfnxcj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3wxtqopaz.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3akocauem.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3kcweible.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3ttelcxew.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3vogsoyeu.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3oqurllml.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3vadnpgqb.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3txefrkbp.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3detezhtk.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3uxdoilye.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3njaumdlp.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3vmgrocfn.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3eptrbufj.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3wscfddpm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3qiclmjqz.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3rqlwosou.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3lyimwsbg.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3emxjqfwz.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3qdvitmah.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jggvnrvt.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3kxohuohn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fcqtnnlj.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ugzelmpp.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3gxcvlqft.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3zmwevekl.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3yzaevamr.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3kqnvybqe.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3kocjklnc.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3tdknpoha.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3ozkvhvrl.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3sxiybuul.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3hvjrlbqu.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fhuyodrq.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3gtvgsxin.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3blsphfzs.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3fsslvgxo.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3lrndlrnm.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3tilbihib.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3shpqqwpq.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3wisviypl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3qluicznc.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3ipbglmjq.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3zeewcmgd.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ybipslzp.html


<!-- 参考信息 -->