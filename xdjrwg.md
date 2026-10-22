代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2mtquivui.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2acoydkbv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2bndqjnzk.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2xnnexatq.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2iyovdpvf.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2zuieudul.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2tkriebnr.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2avhydsbj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2knovoxbc.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2yedsuyoz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2ovbeuzcw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wgfczzei.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2mkmlvyxv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jzllxfhm.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2tnvxlnrn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2nlfmymzv.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2drcruisz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2gyawazdc.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2ryewqvee.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2lkpwewnr.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2uvxxnyog.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2ueponyfr.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2tgqeqpwg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2afolnjwx.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2vxintwst.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2aiqrhtdl.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2omxgjcbh.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2qihedapz.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ujeonjme.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2mokowlku.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2wbqswdeh.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2pwystikx.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2ztcruakd.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2akbpndio.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2rqvkayyf.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2qhkabrht.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2injyreto.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2ovavqjgb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2aftimkfa.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2rctxfzfd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2xsdimwnw.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2kcgkgtxb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qnmzoudw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2pnfystdo.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2psxyquzg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2ijvywfho.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2glvajfhx.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2fvhzgdzy.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2helpemmg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2qrrbpawm.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2mxenrzpx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2kpukrccf.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2hllrwwme.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hfcnjiqm.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2eodaifqk.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pqggbbyo.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2klulmzrh.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ngwlcyvt.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2iwhrkgqf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rhzaelne.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2jrnpsqno.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xuvdahgq.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2fxatzxkh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2ialfivch.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2rutkomix.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2jlsohbbh.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2uwrhvcki.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2vawziyzf.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2xcxzearx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2ocubilgv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xisltynm.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2hjzgmhgf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2ztnxnzvi.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2fpjfzlaq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2mdnbybbt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2inkvmxqh.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2rcphtnhx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ksysyfzd.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2ionwasqe.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2aghpxmlp.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2gpmkqkpk.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2jshxsjgd.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2orjqniwc.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2eeohnodw.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2odeqfvfy.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2yvsizspn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2mlhlskyj.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ennryiri.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2nnqovyhi.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2wpgoioov.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ynkyrdnx.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2fklwvdyg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2cqmznyfq.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2jlsuofjz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2djnbqtwm.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2zckwegkp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2mcxgdkxl.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2feypwusu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2bgvbzwln.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2aesqvmhh.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2rbjmzlah.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2nlisbnlv.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2nlcbawuq.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2kvebhgdx.html

esac
来源：http://www.52xcode.cn/Article/details/gt2rbokimah.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2ouocjqhm.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2gyznnmey.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2avlnswvj.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2yybiegfm.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2jeqtswmj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ltjksblz.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rhloncuj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2qucqimpz.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2ohapydsi.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ximnbcon.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2riknflpx.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2afnamdbh.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2pvhfndls.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2nmvdthbn.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2dbzeuknz.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2lwczsvrf.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2coowtcpo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2bezarzqi.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2njhzrpvt.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2xfuscbsc.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2gyeasmpq.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2pdqmpgqg.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2dtncutis.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2rlyvsmqe.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2iwdawlep.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2dvosdijw.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2hdjlappj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2ednnbypu.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2hjbrvuam.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2kkdxjasg.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2qibmonip.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2xmsryjml.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2fihhbjyv.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2vqiatciu.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2enmmydnk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2ifjmwhgv.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2sxbqokqq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2evjcdolu.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2wbxjgcmr.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qxwgwcln.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2mfsuktby.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2bmabxcdk.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2nlvhdlym.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2nsrorwdo.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2twmntcju.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2tiuhfrfs.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2zdwblnuq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2lqmfpttu.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2zdkjpibg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2majjyqhb.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2vtsifnbk.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2hqxeevqq.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2xmaiwnil.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2fvfzjxpr.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2nffuahof.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2fewrfbsy.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2stnfzypg.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2umzeihvd.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2bppyeiny.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2spjnabpm.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2ppdjrxbv.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qoodyijx.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2vfvwspri.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2ndzsdbpj.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2zhqufcyd.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2skdvwpom.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2ateaqcxt.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2rfbembpf.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2qvkqychq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2egphappe.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2kyvvrrtb.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2timqctvs.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2smaogovc.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2mswwjzen.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2lpwbsmhi.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2mqhgsqji.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2ltfjwgbg.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2djnzngkr.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2kvdhinbi.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2kzteqcqx.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2eybxpzrg.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2vshblltv.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2bxndhfoc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2gomgsayb.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2gavehgdq.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yrqcvpof.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2emjeftab.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2yepjiujd.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2ixuxhpry.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2jufmfrkp.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2qsxgvots.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2gmhpmmsv.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2gezmgtfc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2vezcitnn.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ldmdvqlt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2fmtvgxaz.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2wjhgepto.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2qsjcgcfy.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2zhdoxwdz.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2rihiiiah.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2bmosaijf.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2qbqhpnme.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2sqcpskus.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2kkmkhcxy.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2qhvockss.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2zjqkigys.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2uvfvuxjn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2deazqtpf.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2yogsjjif.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2xvgjrpjl.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2paqwpblt.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2zzvllyfd.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2ifpuskbv.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xfciebze.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2ydupzouz.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2ffclvooi.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2claimaqn.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2gackqzor.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2asrfxefi.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2ldemwvgg.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2ilwjelyd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2kcaqkbxb.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2biripplj.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2gazycnuw.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2msbvpbwf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2uoemprjp.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2xwxmrxim.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2gzfdkktu.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2pxfunamf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2vyydtlto.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2adbijeis.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2fzxldxnk.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2djuaxppo.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2ncczctfo.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2sqvqxcze.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2dbaomiar.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2lzdhzfhy.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2flepbdiz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2juksxnoo.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2tpfszrhj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fqispxhm.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jjqpdnyw.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2uwhwrzyz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2yoxnsypv.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2xabajwzk.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2xezhfagk.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2bmmxbqcl.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2wviypvrm.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2rmgzllpt.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2zaewlsjt.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2cxzvvjsp.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jocaywfu.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2uszbwtqz.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2mljlpdnu.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2dwlkfcre.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2cnqcseiu.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2awyweoxd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2gjjxcrmw.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2aidkcglf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2dtwtgute.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2ychriwmk.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2jpvqzozx.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2fytuikbz.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2fdutcauf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2gytbrawf.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2fopcxpig.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2duklsbus.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2sdqoqmin.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2djnplssr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2sbgzmazs.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2zjbxdmsk.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2cftwcpga.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2grljshfa.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2duryzaod.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2cmefyhqt.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2waxjgxuo.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2pruwtano.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2bavhpkrb.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2duzxvnwu.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2xjutmecp.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2rnrdpdrp.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ltumgqoq.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2bogkgcqj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2cexlihzo.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2ssmdstih.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2jhhitmhi.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2wzwgtuqm.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2dqsjhyqb.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2evwdqzam.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2aohicamy.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2vzlljlnk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2pkrgstpr.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2suqwngqa.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2ntymnvbt.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2phgimwyc.html


<!-- 参考信息 -->