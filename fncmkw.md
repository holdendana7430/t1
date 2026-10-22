代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2uwmulvme.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2aryrnxoo.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2naiejowc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2jngwywiw.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2uojoruei.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2rzonjaln.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2tufvvvhc.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2boozkxmd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2dgvvokob.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2evunmsxf.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ikiiylog.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2vrgmppsk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2uxtvrnfs.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2hwfpthxr.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2uvcadyws.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2pnbnjbqw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ebfrucfw.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2xnykcrzj.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2espbeabl.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2nmhmmrfq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2plxcttep.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2ubemzyhq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2upkikfnx.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2typavmzm.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fsyqrabt.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2xiycbwce.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fvooeiaz.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2kzpmciiu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pkmblxpi.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2tyclropm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2uyrqrtxb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mlzkcuob.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2uevfvnqe.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zpnxxigl.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2wstgdsvz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2htelstux.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2gwkemmhz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2sorukvaw.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2rrtnvwdp.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2qhziqabs.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2glrxjhxs.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2nnmjnhrj.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2fwmwpugy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2vqwonamg.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2djktbodv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2xmatjoee.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2hqmeimod.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2gzwqezta.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2mmpigupy.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2ggezqazq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2ovsvicvy.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2hfcqsuvq.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2tkhgzuyn.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2bdcozbut.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2hcskwnml.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2vzjaxglg.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oqyhxhim.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2rhclxffk.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2xokfreii.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2sjslcxdq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2fxacicjy.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2auhclnez.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ixeuutdf.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2yeteknkf.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2heicvjry.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2ovohesei.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2jdinrhkq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2abpxfzdh.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2akohdwhp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2dbtyspto.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2vojjgwho.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2nysewotd.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2pnnxwsij.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qiciiduu.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2fveuifhn.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hjmvcqkk.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2jsvtpfct.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ekndbtni.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2xqsqzqzn.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vgtrkiip.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2ubnqywte.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rinachdk.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2evvgqrjs.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2hdbpexzr.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2uzmgcajm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2zrbokbfz.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2hjxfhzor.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2rrcpbwyx.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2dfkhfdhg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2tqvytutu.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tgpphmrw.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2mjzicerp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2fkcxjpwh.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2clgdhehe.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2eexdhehp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kmsrbwbr.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2aybuodec.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2byvtnjcx.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2zgkpbfkq.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2nvwlvgda.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2frpmexbx.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2zfyekotc.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2vbwgrikq.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2xkbnsade.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2wneywqar.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2zylvxftp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2lbtuzspb.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2myjdedgm.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2suqmoldl.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2ursjxhuc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2eidozrog.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2veuoiphy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2xzjzuiam.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2hnwaucjo.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2ybvjsmjh.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2vmhueojp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2csjfuxun.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ixfucaxy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2ldzqczfs.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2cgddamnk.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2jwffcqdc.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2scbkqkqx.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2rsvenluf.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2fwsjopxu.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2pspupdto.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2sodjmigp.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hgkznknf.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2vasipxwl.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2atqwarrv.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2hatzbwpw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fxtlcwiw.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2mnarbwwm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yphrjzld.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2ihbrngxc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2wodnzird.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2idjycgea.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2enazdelw.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2ugzqttjb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2dmwlcwfz.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2nfrsykie.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2rzlyrdvv.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2fubvwnal.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2fgsqovun.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2xffbelwy.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2kotzznaq.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2iqgwrxfo.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2exidktgl.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ytxjswav.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2lntlhdkg.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2obajmyvz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2xlndfmqg.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2agmtpkon.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2phzusbdv.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2kjnyqpvc.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2xfwfqpgs.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2yppndjrv.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2umavuhwp.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2yxfvscru.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2ixmlwfne.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2dgzgslgv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2erjcwztv.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2xynzmujx.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2bgiluwcf.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2dfemypjh.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2nmvvfcqr.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2ffryqqgd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2jzttveuj.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2jgwhppfs.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2loinfbvp.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2xqdtcdsu.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2adjmjsnp.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2qktuwbrs.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2kdgzeewj.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2cgkqsjvk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2gssrtyhr.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2pfsocaiv.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2jkqbuzrn.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2kbkbvivp.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2ausfctjc.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2fqstszcn.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2aftloaws.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2uouvrzxr.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2nwpsqewu.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2pdmacota.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2nkawawlb.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2xjjhzdgk.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xfeiwsgi.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2ochfogoz.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2ceudeykn.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2ancxwhad.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2kvezgios.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2qypyedoz.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2cnlevudt.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2ouwjbgbh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2ugldlyxd.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2ugoczqgn.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2boufizjx.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2ktptrnjd.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2yrqbzemn.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2qidckxfr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2owtndtnn.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2xpwgqyyw.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2okoutebx.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2qgwvtybz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2qdiqqeic.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2irofjszt.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2loavusbr.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2qtbjzerm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2wwjksapb.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2teaikzib.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uabvhhxd.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2dhwspmyy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2ogxmowww.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2gqgydjct.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2fowbxmtr.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2xvxmlpho.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2rykawcjg.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2qwzbrhql.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2vjcqmjsa.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2tpekvlhp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2cyftzmdz.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2xnnxvcbb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2qnrlmvqu.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2ktpmtbde.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2rtwpthbw.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2dhyimwye.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2pennnjbk.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2xpqpatrd.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2vkqgemxi.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2zymhynrc.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2ffmfmmwk.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2ounsdarg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2lswprilb.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2uuezpijc.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2qisnbtfr.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2yrvlbrpp.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2tjnjqwwo.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2vdjaogxr.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2xltsgqqs.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2yhbsqhed.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2alznybwc.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2vorzvafe.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2fqgrvhrw.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2eqileqvb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2nkfwybwt.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2mifavdax.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2lzmgsgra.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2flxvzscx.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2rwvpqluf.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2youuskkr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2buchbxze.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2tyvnyzpf.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2vrhsyxvz.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2axxhdaqs.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ddhijpae.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2ounwwnfr.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2qmztktju.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2exyucvgk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2bevphgcr.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2pxtikyqt.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2sqvndenq.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2xigtmpda.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2fhzkmrhn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hlgwpnyu.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2wljyoxcr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ujgdeuay.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ewemnpuv.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2padxghhl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2owdzuaos.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2vjsmnqkn.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2yawzceta.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2xpttyyfr.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2eoernoqs.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2ibsferqx.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2gvhmtveu.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2jnoqhbfk.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dqxxazxj.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2nmkvtpqw.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2haisjtav.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2nyoabsia.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2ajoyjggh.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2wvimgfmz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2bpfnpelf.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2opzbhbqm.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2zfrdfqcg.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2qdntysgq.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2nahtsfuz.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qvqppdio.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2gnlfyxuf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2syatykca.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2vrvopksr.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2mveiylpe.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2phbygbgu.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2khzbrhzt.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2bwqtozfa.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2snfyfobf.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2isxbaids.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2zwskywnh.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2ngriidid.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2gwvowqhc.html


<!-- 参考信息 -->