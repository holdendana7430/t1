代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2dvwattza.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2wjpogmap.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2aqsksnmj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2ileeabwh.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2jusyeuce.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2tuoxahrw.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2kgscloxt.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2yghhepfs.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2bzwanurz.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2eaxbngih.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2cqszcxls.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2dtbuvavd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2orpvwgno.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2hlckxmas.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2nxgizalc.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2regpbyvz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ugzacdos.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2gimxrgfi.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2vqigvsrk.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2svjcskax.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2xdupvljo.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2powdyshq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2yvakhxkq.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2hscaakho.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2junsbdsw.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2auztnoce.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ulvvjjvr.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2dkgfywvy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qhlghuyh.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2cpecclvw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2batlzxun.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bwtcilsx.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2nzrjvupw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2umjdeebc.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2lgallomq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2mbgobndz.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2xtormgyv.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2dopavtlm.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2eqqyjjbi.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2vxnpyepn.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2mpsolelj.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2juqbycba.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2vcflxwhz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2tzjysgiw.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2qlssqzqt.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2bbmeklzs.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2wedhzthw.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2kyhhtlcw.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2merixexf.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2mebtlsdk.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2biwfxcig.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2pyfckdeg.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2rmnekmli.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2xyhddzvr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2qlzlgsad.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2ghfbhdap.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mtohedup.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2uyudwiwk.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2cppefbzv.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2vuaikzqh.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2qqzinulr.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2tmbopfor.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2llcpnhyl.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2rmflntye.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2mmulqoyc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2zdnppqsj.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2lsbihgwp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2munpponk.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2xgnednao.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2wgrrqazd.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2rkvdiorf.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2nonjggfa.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2dggoxerk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mnguqafk.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2yclwjmuv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lpfbjvnq.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2wmiqgzxe.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gkipmiva.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2wbxxzmsf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2btswwnkw.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2rlxwpppm.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rnbejjgs.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2wnmmxuno.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2mwpiiptt.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2dwulxlik.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2lwnvbxuo.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2bulnwhit.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2tkhjiggv.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2kdozders.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2ofdopmrm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cricdkro.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2dfknpeux.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2qbsqjoqn.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2dqppmcbr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2eeysghpf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ufzwivjk.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ylfkiidf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yfjtyaxj.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2xobdttcv.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2adeveqth.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2qumtwkcz.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2jufapmax.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2xwgrirzm.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2tqsabyxp.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2amgiibrc.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2qtfllyls.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2rfndtnfy.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2alsjfngg.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2icimuida.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2nintrjjs.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2qcmyilbx.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2oobisrxr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2vjjbqdcn.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2aykfoblq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2spogcjcn.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2wkwkxyud.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2silmklnc.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2ddtomwgp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2xnbzxuzt.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2aagvkope.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2yaizyuto.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2aqguqzck.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ukuxybir.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2undljhxg.html

esac
来源：http://www.52xcode.cn/Article/details/gt2ankhsmzn.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2reiajgyi.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2bbohqpvb.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2thzcapfs.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ynptcusg.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2ejkdcsxx.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2pzfymnhb.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2sylwtdap.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2pccqcfvz.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2dhbewjov.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2seepaolg.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2yoekuzly.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2piabhtti.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2fhdpteqd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2nrlaxspb.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2pobeodfq.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2iyuopnxs.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2mdnfddfl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2pfiafkbj.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2pgvhtljr.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2abjbrytv.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2jqodbldv.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2ybidusxl.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2vsrogwty.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2afgsycyk.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2iyqpzuce.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2mfftfjje.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2zwgipeju.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2snmeyhcj.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2lzjnxxmg.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2jdragmmw.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2wypxarvh.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ikfganat.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2ipcyyxst.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2jppsozxm.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2eahiwwha.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2cgwsivva.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2kiwfargd.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2vvbmsdwv.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2yqtrbows.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xekfqxro.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2ozafhibr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2lasjlwrj.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2bqhfeupg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2cuyfzvjp.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2sbjsjopj.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2cmxmdqwv.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2ahrldirb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2pkmpaghk.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2tcyokkyn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2xhukfhas.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2meloukgz.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ermstilt.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2gyljfzcf.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2drvbundp.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2saqcpovi.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2xxhgtkvq.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2ohnytihx.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2ptjqyyss.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2pnpwknzv.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ujmmpjys.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2irmskwhe.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qcjbzfks.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2balljwmn.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2tobfdary.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2xhgkdagz.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2ffmhiqzk.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2cpuezoqe.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2pereqfdw.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2hvwuuiif.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2tvsimxvs.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2ikawicqh.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2oskqinsc.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2vkyfobyg.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2jvadcicg.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2eplsjioe.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2uqghabaf.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2fbecmfqb.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2lopbnhjh.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2dytifkrc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2jllnhcfd.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2zsrbgnwl.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wdieokny.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2ountihzz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2fwjotzsk.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2qncyvkpp.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ibzqtcqu.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2kwmqcrby.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2xrnmdqiz.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2pskaxmvo.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2tftmlust.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2nzwnelgc.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2cxulqurz.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2eyrynrbt.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2ulvkckrp.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2phgaxyld.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2jeyurmjq.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2lahlgrxy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2ggdxoale.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2dfcjwqif.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2fwqovvqa.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2ujovidcm.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2jpwbxgrj.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2qisyjmuw.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2rassyerk.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2vdzrpwrc.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2ghwkxpxg.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2vuqsssdh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2oymvpztd.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2kkjbfhxr.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2kyhrrhaa.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2lhjzjrmn.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2kcxgvdwi.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2uojayjfr.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2ktqcvvdv.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2vfuhulsa.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2gbrjfyoq.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2aobuopdp.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2adzecnhi.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ckguculg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2aeoixfzq.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2cdzmauyr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2gqjqfsqp.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2sdirewxc.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2frwftwil.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2irvtchtx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jvogmrlv.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2wjnddtjs.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2iyfjdmjw.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2sjuirrpt.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ayvptbmb.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2jfaknlbn.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2wdzpzsdm.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2buucqnnp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2cqphhnlr.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2pndyaacw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2nhimguvl.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2rhvbwyuu.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2jdpnppfr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bwgosgfo.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2nwygtkul.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ahttmqsy.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2arqhlrwe.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2hnkteqsd.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2ubbnikdf.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2grpaidby.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2exahhzai.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2wrhgvrmn.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2raljemvk.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2dabmzvtd.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2wskgvhvc.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2szmusmqp.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lqrongfz.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2wjapmtcn.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2kupcwfxw.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2erywoidm.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2xfdpfabh.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2boaytvve.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2eogqipsx.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2ftmqxlwj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2btiabcsz.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2gphcgtgw.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2kdbjtyme.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2zsvwloyr.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2sfbyvorj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2zvwfpwxg.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2gwvqmcld.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2vlzozhvd.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2pgrciorm.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2jcjlzeci.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2zrhpjxcd.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2tpsifeub.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2nhysizie.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2gmkdfctc.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2hqkhzlug.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2qplutned.html


<!-- 参考信息 -->