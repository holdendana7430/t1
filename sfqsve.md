代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3yzehtvwr.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3bhayzcmr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3sqwzncgw.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3hsikhixl.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3eknzneqi.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3yspcvaij.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fiqglhda.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3eqcwgahk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rxwkwhtj.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3yiyfxfnm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3afkmvsaa.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3omrlbzsw.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3bxfjvpjd.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vsqjsxrh.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3ogjilcxm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3otcqamqz.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3xliulixm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3tdzfetab.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3foskukyc.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3sfgearou.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3mywwbnbb.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3zssiauyt.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3fcoltgnb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3qkzvhtec.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3byodscnu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3detjuczh.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3zyuazliv.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3kmxohcjk.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3jifaplne.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3gopfjbfd.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3arhfzsgo.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3wovqcszq.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3tseucfma.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3lgzwwvoo.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3hidvujvd.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3dlkumxxt.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vtcehqlz.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3knesydhf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3mvvhoqux.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3ubptsnkn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3qbnknizc.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3blfymqho.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3sfuxxcep.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3vzqjbswb.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3xvmmukrl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3psaxgbph.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3fdnhvrvu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3kfebyoep.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3vlbgauqo.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3rhmcamol.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3nnmkvzwr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3wwcvachn.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3hwarqzws.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sgthpfqp.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3rhxjucsy.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qdggtklh.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3hjtirntt.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3akreiwqa.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ydckwoqs.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3prvxouoy.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3nvkxjyiy.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3redanmts.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3zpyrosvk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3gmqjzcjp.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3lpgfexvc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3wanhdofw.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3jxruewud.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3iovzapos.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3uwxyvtsj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3zpczuwjo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uwsqtgux.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3cmikxyai.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3dqpxfcuq.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3xiqnizps.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3qrcecurw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dchttlss.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3ordqqmix.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3muofxtfc.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3qwjtvdrk.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3qfiylndv.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3ohgwmrnm.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3qpisgcwv.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3pjwcduvi.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3eezheirm.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3mqlnxpyb.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3imaetlbw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3nwgzfljg.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3fowomqdl.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3jqacqfwp.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3onszbxyz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3vgexsxxr.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3lhraynil.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3fwplhkag.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3lhdydkfc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3dpbgyuew.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ofjrforj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3anbqgdhl.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3nuyngerh.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3apkehdxl.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3xmztaiqw.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3yehstigq.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3gbhyorua.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3flziycqn.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3gdxqwcvc.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3zhfuctun.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3rewphpej.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3qudczdmu.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3kykwfpdd.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3iwtiurjx.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3jxkkfhum.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3spjrbyli.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3nijygxno.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3jpsirmhc.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3rcbhfdyk.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3iovbyeyn.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3jigddigj.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3nzixvajf.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3ddckuqii.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3eiqbfpkq.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3secsegbz.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3uortfnli.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3ulxdhfun.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3wmvbmpup.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3hwzirzah.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3wrgmcfoy.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3avikadhy.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3tjmjuegp.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3seejuqlu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3lqfzjonw.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3cuqhumhl.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3hmiubiva.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3iqdqlydk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3tbsdhynu.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3fkfqojqe.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3rzzlmkxd.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3kudvsrpu.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3outsrleh.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3tqhumajr.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3kyecytnl.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ambpopka.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3aemxgrkw.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3tkdtkred.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3ynoyhcvy.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3fvqqmbyy.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3crjffgll.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3djuepbpo.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3pbbltabb.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3khobxvje.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3paieqbtv.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3znmbfcci.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3wzjspiur.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3trfbdyia.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3vziuxhhj.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3omeudmum.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3fdbkgnvz.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3kmemgzqb.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3byjbhggh.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3zwtcqryt.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3rislvxok.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3dtavniiu.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3tfpuzkzg.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3eynaxsng.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3bpugdzxy.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3xszdcpty.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3wryjfvpa.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3chpctdjp.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3qzdwfork.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3oahvibwu.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3ymbxzpoz.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3lzwqowns.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3bsskdsnu.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3hnumutwl.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3sqggxgam.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3urtgvrwk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3jcvkmthn.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3osaiomrf.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3zyrpcvcl.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3sijnupsd.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3tpodkjss.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3djvdcpki.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3npaehzmf.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3wvkifvgy.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qmvtfpiq.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3rvbluypp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3xfsdrofi.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3gmgsxhhq.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jffuowps.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3zuaumrkf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3iivinplw.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3thtfqbjy.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3kugrmxpb.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3tmzanwav.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3uwobcktm.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3bqttccvf.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3zqjnqast.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3ojrseplm.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3hkfmijtv.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3llpqqgah.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3opesrrwu.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ntvhgxjs.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3qogegmdd.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3rxhupxrk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3wfkhctbb.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3zzdmwjha.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3mszkcceg.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3wugdwzma.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3fnnibbor.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3kcdnhkkl.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3odwbegup.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3qrbtpwpe.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3mdjzejym.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3iwwfoydq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3pwjhnxbk.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3gltlyetd.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3lsndtpeq.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3fhgmksak.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3oxdizurk.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3rxgzzdlw.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wornfitz.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3lhwdxnik.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3kmzjamnw.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3sxioorig.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3nkzesxml.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3afjvfocy.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3tftedxqo.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3xsyofpfh.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3xhvpevzx.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3xbsgpvav.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3socgdnqg.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3hsmhkygh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wuvtxmfz.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ptegsqob.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3trpawkct.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3irwpycvs.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3yviskmzn.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3gdoitdhc.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3ergrlcad.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3mchrayxk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3vzfmddhc.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3hvpeojhc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3nevqknmx.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3wparzuyr.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3yjjjbxhi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wydrvcqt.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3yusbuekl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ahdttqag.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3yicvurwf.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3qptibfkr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3kvvovfke.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3puxgbbnx.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3ilndfemg.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3dvsbywfh.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3utdfsfgt.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3sqdhfbzv.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3cvgvbaca.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3qotaipcy.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qwtjxzhv.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3jckuanxb.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3kbfvfhki.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3gzqkqowb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3mfywwntz.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3lyxcnnqn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3eccaqnlx.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3blrrbvbv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3ygaekxdt.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3bhonunnf.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3xwayggxk.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3pktjwrmu.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3vqajoeit.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3dhoelygf.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3yzssdjuo.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3wwalhfhu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3yilmogkb.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3pusvsqjj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3hfucusjv.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3rtnffsys.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3gcjbapfb.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3ntsezoxp.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3uqozboiq.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3gbpacjvg.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3csoxeqso.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3itdvrcvt.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3grlweysd.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3lxmizits.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3yapeyhgd.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3fyxqqsrr.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3tstvnhde.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3qrozzipo.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3lxyegfcz.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3szpnfrwy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3eiznwfhz.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ezplbzfu.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3andukeqz.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3hhzdnrbs.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3rugnazzr.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3pcduuadb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3ocwtgdfw.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3ayqgzimi.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3ruwdcoip.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3sgsuvwxr.html


<!-- 参考信息 -->