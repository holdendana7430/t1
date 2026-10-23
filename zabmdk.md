代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3xgtmcvkr.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3fqspmukl.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3tlvvneqr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3iwwffbpm.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3arkvezyz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3gpjjjhzm.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ztuaiheu.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3paevlvra.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3bqvukmcg.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3wuupepvw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3vwoxpyly.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3epuayowu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3repcpdfh.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3jbpjkfts.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3hfoabnyq.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3jdvqdexo.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3rarwypvf.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3azbwkpde.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3pakydzhy.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3mgjcpqrd.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ncdibjwk.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3mpofskgi.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3qepvryon.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3tewzeoju.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3armmjuje.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3jzjdxlum.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3eqpxfqzx.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3arjjkjai.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mvuxhoot.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3ehfbgdnc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3mteefelv.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3omjrsmjo.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3cisteitb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xbenwnia.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3grxvyxxc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3tddctgqm.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3gmvxnqus.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3rtvdmtgw.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3aeckxpfv.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3offkvyfr.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3wrzvhrdl.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3frmsnpen.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3uundigql.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3wntgnlrh.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3hjfwjvad.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3zrvxtiqe.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3sxcaaktb.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ivxlrjgm.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3yzqtytgu.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3vxtipzrx.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3odptayco.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3notpdqjg.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3hytkxcdl.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3ijchkzxi.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3jkmszujo.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3jlslwtvk.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3aoqqtobq.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3fjzciike.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3ipivmxwh.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3pgtwcklv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3evjjootu.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3dimiyfyw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3goxjzfep.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3xwpbpftg.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3tocaclfe.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3ckvaqdsq.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3fwaiuqny.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3xurpscsh.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3obfkpkaf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3kjultsho.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3zvjsabgr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3xjjclqch.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3ysdpzmbs.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bitnakpp.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3rywwjdyk.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3unaaehke.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3rnxrorzd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rfzqycaz.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3gtkzyrvh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iizrtyro.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3bjorybbo.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ujhcxfat.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3zytyintp.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3ukuxdiio.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3cndeculo.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3chxrrqjw.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3bufgybrp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3qemdoqbu.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3aqwomivp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3kcwpzfkv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xyksnwds.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3tazmabab.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3nexaflvf.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3dbgmmoqs.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3sztupxgg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hqwuiqsl.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3kkvqflfb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3agrspebe.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3bpbxckwx.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3jkhbyzqz.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3tqnwturw.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3rccptpqo.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3arikslux.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3tiblnefv.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3rybqfzjo.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3wiurrmbh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3mchntoau.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3kpswwgnp.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3nbhpcgtr.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3jaaldoly.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ctgiilrm.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3ivrydhhl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3kcyfmsrm.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3yfgclchk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3pzcibvmm.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3bmolngfa.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3teqnnuiw.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fpudsoej.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3emiclkbp.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3daguewab.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3nnrvezpi.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3azctlapv.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3wwbzzziz.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3avxfakzy.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3kdahzlmh.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3lvqgbndq.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3smaaeupm.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3abhqanhv.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3vcwklqfx.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3vvxgeuhu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rufcqpmo.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fmfzlkyd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3cgnldqtv.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3colaubhm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3hafxgvnb.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3lpvhvqlh.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3zrvwdjfi.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3lxwkuvfj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3jqybkamt.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3kcjyehid.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3hkiulzxt.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3aackwxkb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3oedjpxiq.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3cqsldsnl.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3evrpatcq.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3blvsdsdg.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3tbqirkfg.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3iyokgsyj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3zhyndkbh.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3xsiesyic.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3urtzuewb.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3ffcjnlid.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3dzzpjoen.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3knivqgjm.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3wzxgsfkf.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3jtazxswq.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3itqesahe.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3xagnwvyv.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3lzodsynt.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3fomhszow.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3xgkjwari.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3ngnrvhwq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3zqqenzpe.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3nspppxno.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3gdbfrkrw.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3dznwnxzz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3vlwwyjdw.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3jphgtddm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3cjswvepi.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3ddqljgjg.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3uljvfada.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3wdvmuiah.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3orpugmfw.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3crsqunrw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3zswufyog.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3gruodvci.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3lbhvbtwv.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3qxznfyrz.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3amssasot.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3ycigpfva.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3grrrxnod.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3umsvfypu.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3krfdswks.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3yvzlvhua.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ybbhasne.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3exttcpvr.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wnjekgql.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3iqedmxpi.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3eruibvkz.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3mxvffbbd.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3kxfandru.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3usviihsc.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3fpgeuyou.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3ysbceffs.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3lhwljvkb.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3awpejpjc.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3qyegrctj.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3xcdqamun.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dxevskks.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3uiudmsge.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3ksvhvgyq.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3wqpnbqym.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3fewhiqlv.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3fwcneuiy.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3augfebse.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3djqcufwq.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3hgaiuelt.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3objdrsnw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3kxwoemsh.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3tgdxajxh.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3ufbrbrgt.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3qcfmgvkr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3vvfddthh.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3azudpenc.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3zlzcabok.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3tiafeqbn.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3hryfzatu.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3hevtbuhg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3fjioibgm.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3zlohupze.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3nhipbgzp.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3qdfhaabf.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3lomfhemh.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3ajeuijww.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3jagijzih.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3irrrrtsm.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3vgltonuv.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3pdvpuply.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3ftmfhwut.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3qydepzlr.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3rfqxkxzq.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3vhpoqjiw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3mywdlhan.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3zcnjfhqw.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3adhfgpmx.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3njnsgqsj.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3nvsdtdlv.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3gohjfxsp.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3xdomkqca.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3xcqvhxhc.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3sdqflhmj.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3yxbxlrxt.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3gxcwsqai.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3lhbemmop.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3xysqxbtb.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3ngyhljkt.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ptrhykrx.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3jxsachjw.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3dpqgucxn.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3ypzhvvkz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3cwbvdelc.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3despnnwv.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3gfidvlso.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3gimkdmaf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3fnqayapx.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3hxvcwert.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3oqrdkznr.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3bwzzrhvk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3gdkftjzp.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3aspqtfsc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3ogeyqmuk.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3sibjjvip.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3uoedzljb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tqilqkkg.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3pumiizac.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vupuvqcp.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hnbxuops.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3aguskede.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3bubltkot.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3ekpjturj.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3fxerzjcm.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3xjrmtrsv.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3jwhtniqe.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3sjcjpfci.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3fyvxgrcv.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3evlmobro.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3kzrbblwx.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3qqzuhjco.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3olgdhols.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3kegqiufs.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3rrxapbrb.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3xbpyabkx.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3sbpczwte.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3dajlspmr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3ehpkkjiw.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3wyyiqbsq.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3sdcewooo.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ebhewrid.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3slnvizve.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3gjchimni.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3jsenizqs.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3crtbhugi.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3xsiiasye.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3zrqaycma.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3klgihiqt.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3yxxxbrgz.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3uvwrdoty.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3selvdczw.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3tmgwvejl.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3kxbafzsr.html


<!-- 参考信息 -->