代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3gqstbhht.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3wfmxmhrr.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3tobmdfrt.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3fkdmldmz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3nqsrvipw.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3jtrcpjtz.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ohphjftb.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3rdcmdjzh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ysevvlrk.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3ynixtfqg.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3mnrbbgzi.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3kqbtcmvu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3mjwendoz.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3xoqqknxl.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3juiqfcju.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3dhybjtfv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ydcggteq.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3lsmohzjf.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3myrnlmgb.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3ogeadelc.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jojzahxz.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3ebzqpjhm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3bezdmjzn.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xafprfnn.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3nkexcwyj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3opnudwsv.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3ttyvsibj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ickcpfyf.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3eymygoyp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3jisrlivy.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3judaxyui.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3ogpamylz.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3wstobpvv.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3ysuvgsna.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3bltwqwbb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3dietzdqh.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3xdelihrc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3jqopptpr.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3faiyrypo.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3zjktrcip.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3pgxdpyph.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3necqssgi.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3ostdyzbf.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3yhcegkuy.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3clsxorhw.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3gkppcofr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3viavckjb.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3uyxbxict.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nrqsnhsl.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3wrikcyiv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3dghjdsqi.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3wzanyfrj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3ojxpehju.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mpxqmidi.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3oufkgbbv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3frvfrprx.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3eevkoexb.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3ydnweosf.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3syyyvrho.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3thalbcqa.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3zpdchqob.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3sjmqcncq.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3hmnyswnb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3upxqqkzk.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3omxslmws.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dhbyqxva.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3pnxcgneg.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3spzwlzsx.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3qihtpktt.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vmjmpvjc.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3iaxsygwr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3onznzwan.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3zwsyamfb.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nnylseik.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3dcmekrnb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3wgmypkpt.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3xvlskxif.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3rejxmlqw.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3ktdobscq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3vpnmryoh.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3xlwgwnif.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3puesyclq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pfjlknni.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3vobnvrfj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3ztopxdds.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3azgywqze.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3znxdaatw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fitfimay.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3zkffkhpr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vnwfbqna.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3xldqubyd.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3zigilzkz.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3trkexhin.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3owqbgctk.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3lqkxjkqn.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3dwjepytt.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3pneuanki.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3qnpjraur.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3soekwtwk.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3xvbcekqe.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3vhnxkguc.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3tzgepzlh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3tgoaxtym.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3duycqzoy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3glnukaaw.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3mszpozez.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3ktcegyuv.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3dydfvlke.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3pdsgkobi.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3avklrmwj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jtlwkxjp.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3dvwyzsjp.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3jqsmmdba.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3aioyalij.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3mortuvgk.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3gdqdgoni.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3jqgazvei.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3xjpazmnn.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3eloaiknn.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3gbwinkgq.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3zfwzjeyc.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3upsnrobc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3bbegamnu.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3qmuzhckh.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dzibkewe.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3fmpbmnxe.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3mhlaqbwc.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3qviycdsq.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3xgtuepoj.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3xuujkopu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3bqqdzkvi.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3zvhjjnsu.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3qtdvzkds.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3iezmywwe.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3nhaxcbkw.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3mesvpfpe.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3yqhlkwqt.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3tbclmktw.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3nhxrwytd.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3fdlhqqhu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3qtmslxrv.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3nuwdzbsp.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3zjgdgtek.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3iyfcplra.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3fgslqrlh.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3srwybqaw.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3zzbnakqr.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3gprskukn.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3bbtaqafo.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3jzhidfod.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3zjikbpjr.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3gufkpbuj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3nyfpkxut.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3tnpwfmvp.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3zguhztpv.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3waotonwf.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rubxxcqd.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3aokpjepi.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3kokhglvw.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3mcmmyibg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3senndjkm.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3uigbsvuv.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3ahmbozsl.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3aofdloyh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3sswfrzkj.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3dwfnpnnk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3zclxudix.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3lxyktlef.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ehetfpwk.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3rudgbnwn.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3wdkejzac.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3fzqvopsp.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3njgapwqu.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3dbqgtpxx.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3mieupjte.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3jxtaevag.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3iqtnwnsq.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3chogscnc.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mvxidzxv.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3dodjkdcm.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3lcpczlku.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3bjkuyjyx.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3ronhpkzs.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3evidnnlb.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3xorqnlic.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3nqaevgof.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3islvlmkl.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3lsfvlhal.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3laxnsren.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3dluefsdb.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3lespsgfw.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3zsvczuap.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3efgprfhg.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3iioaioof.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kswfkgeg.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3yysywbke.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3cmqfqnxy.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3mtowzkcf.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3atalvodl.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3fzvryovd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3fgnyxzhu.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3sxkxuysb.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3defbcmjv.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3rpvspzvu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3kvnvhevk.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3gsmsusdq.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3ysjizzmx.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3kpjxlnxh.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3gzuztppc.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3brlvzjvl.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3qotpiqoy.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3jzjdhmqd.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3daavwywn.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3zdolijwv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3sqqhpolq.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3rsqtwoqe.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3iaimjigm.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3dqjgarur.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3nlgihdtd.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3mbhotyfu.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3ihhxjyhc.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3jyjeawtk.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3skszyeqx.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3ozvaptqp.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3pdcblpii.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3aocwbpys.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3dlpibvxr.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3anuetggg.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3kpdqykie.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3flqxbnxo.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3gxuwqncj.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3nzovzkyx.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3qixcbuki.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3whpuotno.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3midvbxmo.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3lqihagxb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3rkxoxtql.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3ucfnjwua.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3hyithomf.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3vqetilsr.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3zpfqhhuz.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3upwuqrfl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3atigqeay.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3uqedyqfk.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3lspddwfl.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3jlyxjxgm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3emwbsqfh.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3hcagvdkf.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3ljqqxuuy.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3vvijssxm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3okfydjms.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3anumzpxf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3jiqyiolo.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3osjkxrnm.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3hejwuqpc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3avwwwuuq.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3gzxhgmwi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fujpdrdx.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3crpyjfkr.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3rxmjnipa.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3teuamrsv.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3pwfuamdj.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3udzvzkkp.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3xbxrzckv.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3pqtpjeij.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3sknrnqgs.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3lrkoorpp.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3xgfvrsjq.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3smpbrzay.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3fbnzvloo.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3ekhlynhd.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3bussnfiq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3hrdcwqow.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3mrwodzsf.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3pebpiddu.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3phqbufug.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3pdgpscpm.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3eusntxur.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3paqxwcmc.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3wxmkncbj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3xusiiddp.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3iqzqupvx.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3qjikqgtt.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3wmowplte.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ukigabzf.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3xeebiijb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3fujpcfmy.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ddqgsknv.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3sqlgxxxa.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3bmtyablu.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3rtaxoqgv.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3cnkkeqhb.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3likxykkx.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3coqsqfqn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3yyijjajw.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3vjymbson.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3eyvcilch.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3fmjxwddn.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3orsbzabn.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3wvatxsju.html


<!-- 参考信息 -->