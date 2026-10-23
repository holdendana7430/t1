代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3zeruiugl.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3fyubmvnb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3cupqbsmf.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3fcyqlbbb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3yxiigfcs.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3gibrsnym.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3wxzpzozw.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3tmvlbdte.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3cjsmnmwr.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3dcpypbtf.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3wboqvozr.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3tgzlzzzh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3xvoooqll.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3wkyffaab.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3johkujli.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3azfwqjzf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vpburpvl.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3crktxcte.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3asvuokov.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3svwmnldc.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3lpwezncf.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3fyprynji.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3ikjdsrgx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xxjuhfxw.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3wscikpyy.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jduddneo.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3yypakced.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3idykywcg.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3jqzqkubl.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3zarbaclz.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3imlausac.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3nojbjpvf.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3eixwvckn.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3juxsfwxx.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3rhiyaluz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3shbpommw.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3yzccuwtk.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3lnrfrpmm.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3ospsytzw.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3bhyosxyu.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3nbfszbjn.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3oraxuosj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3ohkccnup.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3nubykuas.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3diqdddbi.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3jhfstere.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3zxpwddvd.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3eosuprtc.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mktagzpv.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3kqjdoysj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3jdqgknyt.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3hqdhptbr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3mihrkhfe.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ulkwglwy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3iplvexvk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3vyjkymvw.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3zmkpprma.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3bsubdvsa.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3prmscfmh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3iynlvmwp.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3qbsqfeki.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3eguwgkjp.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3rncalsfq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3mbveuazp.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3rjwqwpge.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3syphvmkk.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3jqasaqeh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gfmqfizu.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3vblorssd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nggnmtqy.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3rmynydxg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kliltjys.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3ennmmfqo.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hjgnfsdn.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3exugmafz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3vcgsfncs.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3ytshpwex.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3lrxycyen.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3alwdebwt.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3hpsifzpd.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3wixvhtno.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3zomeichr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3etbvtpff.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3pxnaozjl.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3rpecdgxa.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3nfraygml.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3xhqtdsua.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3edlxcaea.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3naaoojyr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hsioubbm.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3lnzutmrf.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3hxiqzfvf.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3idmzsmmm.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3qctialzv.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3qanonjau.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3czudpxvv.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3ktmyzqtz.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3xxycidty.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3qmnslzzx.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3qwktilxx.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3cspddura.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3wryvphbm.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ozktjmqw.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3ndhzdfhd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3qtftbisq.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3qyrwevsx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3gqienhqd.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3dorcgzxe.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3bytkfeaz.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fegbakup.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3xjfmdvev.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3qyngonjy.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3cgafykuv.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3sstedcso.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3jfoeoauo.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3qqkfdpkh.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3jjixdgmj.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3vxmdkrqe.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3npjzmqgy.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3iqqfgswo.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3tadwhwnf.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3kqdxvyzu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3nbsnsnyb.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3veoenmeh.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3iihehlre.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3bnhcwcjf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3owhfzhmv.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3bibebywl.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3ctlfxlwh.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3zlrsuamf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hdnuxzkm.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3bxrvasdq.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3elhdxswl.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3ygbcjddl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ahgddeql.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3sxrykdkw.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3lrdklkyk.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3tdvhkenc.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3ymdjqjgk.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3npfksvnt.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3zgklepyy.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3cpdcrcol.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3mmhejmgl.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3pjnaqhnx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3eejgzrjh.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3hquhxrkj.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3jlrfvqcd.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3mjnmncor.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ynffcigh.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3wzkekemp.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3wdhzjgft.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3gjrgwzib.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3kijbeovj.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3prmszwqw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3ddekhtes.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3xfsqottw.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yjywough.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3gcghgchd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3vcktvwwa.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3fpfnifku.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3nqortuiy.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3emwvbvol.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3odlstwsh.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3ihgkyczu.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3eqyjxhiy.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3gayjvxvc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3xpiachbw.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3kiibevzo.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3bgalgcaw.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3cwciuhhz.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3wldpgfwf.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3bzeatbho.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3yvjgiluf.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3huhzkukp.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3tjjzwtgy.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3xpsxuhje.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ltsyqech.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3xinokedg.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3rmxvtenx.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3dquqprrj.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3fyiqwczs.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3fmsmyido.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3snuyndmx.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3crltnzkh.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3gwchejsx.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3iccwkapo.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3snbgwsin.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3fbrywkpj.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mhgryked.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3bxkwnhds.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wegslmoy.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3xtgaehfc.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3fuqdurct.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3lwcannzy.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ybbbccpo.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3szymcggp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3hzvtrjxg.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3urergjph.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sauxxcco.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3lefqvbcp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3dvraugvh.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3bjqnqbqd.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3sndqehck.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3kqmwrngf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3swkmrgdc.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ryjwivip.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3quzncxnf.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3kuiklrhc.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3xgqpkaze.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3oimgcdzw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3vguydgap.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3aldygsgm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3mqineguy.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3dubhqric.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3btggtbor.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3uhsyjexg.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3lcsyzook.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3nugokzzo.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3plwtrknb.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3xnitvxgz.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3bfetmhii.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3leeebvnm.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3kfvteivo.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3turcombx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3flfibbxc.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ggkpenfi.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3owvcgdig.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3jdunzkjt.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3olnqmgwm.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3myhsmhuo.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3bbrkhxnn.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3chkguxws.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3vbccgiqa.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3zmghbfyb.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3svcntmcp.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3whbsqniu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3erjoyqdn.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3ypytfptw.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3yblcqkpn.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3vsnvlkvh.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3fqvbokrp.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3ytyntldu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3eljdxwpx.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3llmaitrq.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3bdtnkibo.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3kntciplm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3cgmarrpg.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3zkdveizu.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3ewrxtncp.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3wpmwlzdi.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3vzeyqdmo.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3lknxucbw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3irpaukmv.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3wzbblinp.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3vjyxxxxb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cyyqlrnr.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3uycrrkay.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yfngcpcv.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tqmkjuvq.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3plqoyqsh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3fnuvkyam.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3ikmecwvg.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3lakpulmk.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3rhoumrvo.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3rqumdmct.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3dpwvmcfz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3kckvxjzd.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3sduxnzgz.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bqfvjcuv.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3kqzxjlkh.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3pqllpqgb.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3kgpinsks.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3lcyxwpxm.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3pxavegck.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3blxswdqy.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3ziasmqny.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3avanuyus.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3vwiinssk.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3kndukeuy.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ajtpmthy.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3irjipevq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3nsrpcdpt.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ggwhwlpu.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3kpawbdkj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ozywzncn.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3trgqzqin.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3dkrnlmyq.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3bhorkogq.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3afbjtwam.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3nggsxlyx.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3lxxqgqeh.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3kescuukj.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3uppdfhfw.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sdetzvsu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3xuncnpxt.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3uoswovbj.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3ivtgwsqc.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3bynpxvcx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ijmmfboe.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3ckzipctx.html


<!-- 参考信息 -->