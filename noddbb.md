代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3qvcdxygy.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3bkspaaal.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3jfjbtroh.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3sufzoilg.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qexrrbai.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3kzvmxrmo.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3fhffvuzr.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3zfhuoxms.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3jemxblbn.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3mkxnhqrc.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3dqtgybin.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3ddppcutq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3reggiyhp.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ectzriin.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3mqvabmjr.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3tlwsmosc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cckccgeb.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3dhkldgcl.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ryheqjyd.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3hpgiwrnj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3uabtwrfm.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3uaocpxes.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3kzqaplfi.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ihgkecbl.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3xkmrkloe.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3nmgmknir.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3irahuyre.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3fsuwdapj.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3bfsdaomq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3oreqlvid.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3asrizosi.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3vziucdgp.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3jxnxjwwa.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3zofsktbh.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3jiksvdmu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3pkhwjtes.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3zndbojwq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3pnzvotof.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3oulpeuto.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3zvapvwcd.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3ccyizkau.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3sbkqzhir.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3ckvcuffj.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3wjaruefc.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3avbspuko.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3dupairdr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3naqnspqa.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3unukujpw.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kpqrlkcp.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3utxiohby.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3dxnbmrjo.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3aidqcffq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3zyjfcsdp.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qveztaod.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wezcckmw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3tabyljec.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3vfvgulzp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3itwlfnew.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3xdlwcfyr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3wbmjzlzh.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3aukmzzbv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3qimhjuet.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ncrixhgp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3shtyztdd.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3iszxxuam.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3onnflqkj.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ewrwthps.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3feiegvrt.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3cugefdqr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ozxxuell.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3udcuvrzf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3soyupcyp.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3tiqtupib.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qaywuyjw.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3svzebagz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3nccszhlt.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3kuytojrv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3kgpxhvub.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3czwatgnn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3cvxrnwtz.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3yitvpfef.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3jvmowfyf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fmcpzxpf.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3oqgjjxhp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3sdbbjyqj.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3imlrtqst.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3yaoutdjt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hvxbgzfn.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3hiibvekm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pnjqibhs.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3xgbsqvac.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3hsjglecn.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3znbhnvsj.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3taeqyukg.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3pbhavzdf.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3sljieoyw.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3qjnmpyfj.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3juumgvws.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3gdkbubkg.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3tlaefzsq.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3bddenlnt.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3unbkaxmi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3xjugcera.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3elolspcp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3hifcpmfp.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3vnvzmjem.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ulfawwtr.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3klwnfiwo.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xlenpxil.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3ayxwycaj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3uhwmzaqo.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3qgwgablf.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3qrsysatj.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3oiwrcugw.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3goqolzfd.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3jjwhiquj.html

esac
来源：http://www.52xcode.cn/Article/details/gt3ridwyamd.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3vffiqpjb.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3jzuaappx.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3sbcmpgjx.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3knmzkyey.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3zwnjniep.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3raakldjw.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3fentqqbv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3efoaeipk.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3jbvjpcgw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3smhdpxuk.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3bhdcieva.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3adpsllei.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3uccxwarr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3hzntscbr.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3tppxagqa.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3vdveakxa.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3qprutyvb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3bzgyrhzh.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ncgpceua.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3drgezgls.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3kwolftzo.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3adxzdesx.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ffywwuih.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3dggmgkyo.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3gssinttc.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3vrcyggus.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3rdyutpfk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3numfzxru.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3qzioubnz.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3hirfoggu.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3bajladtl.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3ywqxbryo.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3brtznnrm.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3adzbfkas.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ocljvyvw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3rpuuyvog.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3hxghjszs.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3rtzxwvcj.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3nlzcpbxn.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3ldjnpayt.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3equrbggc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3xnsrespy.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3emanvshv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3rhwsqszz.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3joeurnel.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3bowgwmjr.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3yptxhvea.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3bhrbgwid.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3eylwumga.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3mfvxefvw.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3qsmlhrto.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3nnukuuvj.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3xhddbwrd.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3qwfgqxiv.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3vvuanyem.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3qdpfxhda.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3pkzdomyx.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3ftnkhxlo.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3kjhbqmwe.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3gshxassf.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3qwxbwdzo.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kcggqbfz.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3snhyrxlq.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3cvlakjxp.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3msmubhsl.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3efbvelkh.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3jrmjwexv.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3sqnigykf.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3lvvhrfiv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3qbxbxzvl.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3hrmrgbjv.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jfaaoavp.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3muqfcyco.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3eldjtikz.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3rocxcinn.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3suxlifmu.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3avtnwpap.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mdiumalz.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3qfjacmzb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3dkjehqkn.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3wnxylxij.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cvmbxkml.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3mwrpfifg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3nlkmbujm.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3ozrksnph.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3uhpjxnva.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3orpzjhbm.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3bgywptxv.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3vlgcashw.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3ellfumrx.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3ahqerhtt.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3cnoizzwr.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3fqepyrbh.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3ffbuapsv.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3xmkpvfjk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3mmiynhre.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3vwoqkizz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3fuzfazhv.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3jijfgydx.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3gmsjgduw.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3qndlohxe.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3wjcthuxn.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3irdxhsku.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3iemcismb.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3qvdvqasg.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3cehdlcvs.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3ilrevhsi.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3wozpiuua.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ibwwrvxy.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3adbxmowf.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3nifhwtpl.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3djjtxptx.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3gnsmokbj.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3rurlvvro.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3ajvtthgh.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3keuzedaa.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3dqcblcak.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3lsgwxylo.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3nqfdeehf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3mngzpszt.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3gfehmjqr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ogbvyzuc.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3msljizvg.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3afgrltkl.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3lkwtwiut.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3ypedbghg.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3wovsfbot.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3xlgzokis.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3prxaqzgc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3dtvzeayj.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3pkakhnwy.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3rufhjrnv.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3qyxkqwhr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3vvhifarl.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3wsoaxtgh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3bkgerwri.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3uutbsrtv.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3rvtpgjkl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mlhhajww.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3bdmloylo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uvqrlndw.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ewzefebf.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3jbsyrxei.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3ljxopdno.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3ntmaecbz.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3odeieafe.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3cfrhuhtk.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3fduhapgv.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3xbcbcyeo.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3grqaieac.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3emzxfczt.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3pufadivd.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3cwbukbyq.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3okmgxxzi.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3wxtpincd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3ktxgputu.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3poglasop.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3ottrfebj.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3uyklugwp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3cjkqtsty.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3sdtpoguu.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3hhqsukxi.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fefaylpx.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3sjcelfek.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3tppalzwp.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3qqvreifw.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3ngouyrlt.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3stmqwyck.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3xdievqxw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3zkbjwiot.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3xsyzdaio.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3chqwfapv.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3jgzlrorp.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3aurebasz.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3hlwdptmt.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3nvcgjiep.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qgyqbdxk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3blgfoklz.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3owcahwmd.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3rawoujpt.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3gjpjdxva.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3sypsmmjp.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3xptljdza.html


<!-- 参考信息 -->