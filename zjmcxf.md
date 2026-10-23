代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ktxijpll.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3yzzsgbzu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3yblmkshe.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3jyxwndjm.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jftbtiqu.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3estxfqip.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3oazivkvq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3nbuvowml.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3gojlpbyn.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ednuegpo.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3ztmsnezj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3uopmkvgt.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3uudsarow.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3tbhwzyop.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3uwkfbtfq.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3ytjtxpwt.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3afwytxbd.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3ngrczixc.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3hlvsonva.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3feoetddz.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3znzsebcn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3rwoeewtq.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3xncyapqq.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3ycsgxbtl.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3qzlkmhps.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3cdxgvjlz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3emgbicdo.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3znyxjtmf.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3febbrrlj.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3zvtzydya.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3xfxlqlnh.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3fbnknlvo.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yfouvnwr.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3zjihceuv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3bdrbeypg.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3nlfdqfiz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3xurlifut.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3omgjxcqg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ecpfgiic.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3uvegckuf.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3xyurzqme.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3ztmngbfv.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3nsqiyrlm.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3bggbbvqu.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3jzioohdy.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3ganrhwjz.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3dhybksvm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3wlcacgwn.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3afhbllxt.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qgvxbnts.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ojdjgkix.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vgwoannx.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3nunpqdln.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vaeeglek.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3wfmtvjpe.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sgeoahva.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3esorkvzh.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3glbbbwyv.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3zodskher.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3lusgutew.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3ibunuens.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3wclyuaej.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3lfdpgddl.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3fuweleas.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3lqsaktfe.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3ncrztnlo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gzzgcmpm.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3zkyyayux.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ueimorah.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3fkidihxw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3thorfrqx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3alwlxsln.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3tlvdwigw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gmtphcqj.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3zahrglmn.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3fqdytkpv.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3zhmtnkbm.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3jvyqoyzg.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3cksuxask.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3xqhpelbf.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3nujkllsa.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3tudmrbqa.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3fhlkqmpm.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3guurprrm.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3qjmnkody.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3qelykouh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3rpocjfkc.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3yatljpgx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3vjggmmta.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3xuyltisj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jmabcxfp.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ckdyoccl.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3zoybowfj.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mauraadk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3lsfhelkc.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3hwxpxkhi.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3uxvpzvsy.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3chusclxf.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3oqrhuvgw.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3dtienioc.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3fausfnsg.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3rjzaupxj.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3inoixsxw.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3kvjxyyvn.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qurfxibz.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3rxodufhr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3cexoowtw.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3oexvtksn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tyiwekxg.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3vgpaesjg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3vaavxrbx.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3iiazoaiu.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ubephrif.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3jearjubw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ednzdjzy.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3cwtnqbzx.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3hgjnwdca.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3onjvlovh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3utltnvfp.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3qrmiziax.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3gzibpuob.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3laiemmam.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3fuapklpd.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3yrbklkmy.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3kktnpzba.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3uegqgkaz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3jxxndgwe.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3fpkzlegk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3nqdywpui.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3jibdmexq.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3kscqnrjj.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3iaktxanv.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3pqbjcwdk.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3keflltfn.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3laglplfr.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3jqwwldic.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3chcgnbno.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ngtffanz.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3peaphboo.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3sbjtuucr.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ijkiaawt.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3tucmrzjr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3xtqsrebp.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3mvyuomhz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3rirmnduz.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3zoeglzro.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ynzzuzol.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3fjbruabn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3cqyqcfpo.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3zwztrnua.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3fvtqpnwr.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3uwsaksjo.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3iyrqdynp.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3dakkrpku.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3tcxedtmx.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3alrjyvju.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3hrgrpvmv.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3hmxwaifv.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3dziiohdq.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3rqvtebhp.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3rezuqryr.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3zrsikcmn.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3svpoaito.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3ojkyxjva.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3ddgjaxdr.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3qcqcfbud.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3rqrqlzzb.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3fojgzliu.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3aywhafvp.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3nssomypt.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3odcihnmc.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3vgyvcjlx.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3eukklcor.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3viqfkcjl.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3tozfrgzo.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3ybqbkwsr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3fxxwclkx.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3srqwgqty.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mpxuohfl.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3lcyddeqt.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3hptdeypz.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3bklscvtz.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3mallzteo.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3fqktsqwh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3nweiksaq.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3lslqxagf.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3bcfsrwgz.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3lagsaysk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3qgahgwgw.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3bsqafqwk.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3vaeyalmt.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3eojoeieg.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3kdtmjcqv.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3vfyrzahu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3ueuvmfan.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3jbuyayml.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3hgkxmxgq.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ykrhtqyk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3dqrzpfrm.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3mxndfoqj.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3frkbsdvy.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3evmhtkry.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3yahlvuqu.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3trmhxfsi.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3oschgkdg.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3vncdnbju.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3htrejfxi.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3esqrlczc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3qucvaxux.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3jzcdrktf.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3vmevcrxb.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3adgyxevg.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3hpdtqmnl.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3nchzjocg.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3krbfpurh.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3zvevrlaw.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3bohnuukn.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3qwsxffyi.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3sslhqlrc.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3krwbndlc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3fqlrnklz.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3gvlsqyey.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3okhmpciq.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3kuohhygu.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3vjmnnjrq.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3pbvexyww.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3pseovwco.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3bzoqikix.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3cnwkfneh.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3flrvznkr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3yoelnqdn.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3zxdqmznx.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3vhiwssih.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3byagblqa.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3xhaiggef.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3mvhherok.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3dgqbhsjr.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3kfzkwysq.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3tlkerucm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rcggkdbh.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3qiphrjkf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mzlkjhew.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vjytwkxd.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3kqgyyysy.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3bswhnpvt.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3iuwlgmkz.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3yiipybwm.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3iyfxalpn.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3lafjljsn.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3scxbcmqn.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3pnfffxwz.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3emonaybe.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3awjeppae.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3nrprksmd.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3opaboxnb.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3lefhjfxg.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3ecsnkbzg.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3eizdfpxi.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3vtgrdimi.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3jpwzzuoe.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3dkanbwkw.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3qrbrmtxs.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3lhxoeqmq.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3zjysydrz.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3qjehdoid.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3aoqjgfzd.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3riuowfou.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3rlxhlwzt.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3usmkxwwp.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3yxjnlgfe.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3wcdppaee.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3xbvywpar.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3qtahnsip.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3odxwaibr.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3hrbxecxv.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3yzbglzeo.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3suzixoyp.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3fdffdohm.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3apwlawqd.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3iustkled.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3edpmpmqr.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3huupwudg.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3capcmhkn.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3wlhwwsfr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3czcruyai.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3lxfcghzz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3drozpmeu.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3mirewgqj.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3liotkmmr.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3huwywiwi.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3nupbihmo.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3vrvsxzty.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3xurzpczd.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3kqtcohoz.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3pypkkgrv.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3nhkuexeb.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3nswckhma.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3lsswdpgk.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3msudvbkm.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3odncdsrz.html


<!-- 参考信息 -->