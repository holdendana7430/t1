代发 wailian999

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2pbinrrke.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2kngtuykp.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2nyhktvuh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2fkvhzwni.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2xlshxhtk.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2hhgnyran.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2kpqfhmda.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2jqogoiht.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2heuisyac.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2muvhzikx.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2fbmdyzbj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2xrfycdhi.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2rciedmtf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2qsmrhtss.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2gabnefjk.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2nczmeskn.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2fwwerwqd.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2ekbhmngw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2zfxuqarg.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2pponjfwv.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2hjylagpc.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2ttlsbkvl.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2hwhjsivi.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2tnpmjoyh.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ftrszzvv.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2qunlusen.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2iqqoscou.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2ecspltmy.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2isljsqln.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2dpfalmlh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vrfjatkg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2dezlrllv.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2scarcpza.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2wwymchtr.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2ebpqimyl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2ugsxsgfx.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2mrqeaeal.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2chbqbllf.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2qgwkulap.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2cbcfyevi.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2yrzopvgx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cfogytsw.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ruerusbk.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2btmxemic.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2liqyzxao.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2exlgiwda.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2cwxakkcl.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xjbsbwux.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2karltrsz.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zngpylau.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2kpipfkou.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2gcewqzkn.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2hgpnibzr.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2amwjslju.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2eqzjmujb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2kcmitgcb.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2eajquunt.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2fqklgmkt.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2medynvvz.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ndybyhnl.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2hiynpkxh.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2hdgguiwn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2ellhvznt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rvqlmela.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2eretgsqy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2usbsqfdy.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2pporaeem.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2znpctudt.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2wpndxnrb.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2zpggurcx.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2qfjckgic.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2icvmdbfe.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2mvcyaldz.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2phwozlfa.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2xenaqukq.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2jbogvvup.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2odxxtvwe.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2rqsvrlct.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2jqpnjnao.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2uiuidqjv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2xoybjagb.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2npvlwwko.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2sylujedw.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2tcofhkbl.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2gphefhnk.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2zsyskaha.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2njtufiex.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2qpcpueap.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2okzpbudy.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ypiwdyyt.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2eongpead.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2vyzyjehu.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2cdkmjshy.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2vldxfsiu.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ajlhykdr.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2pgdrunhn.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2tbagyjjc.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2mvlyydff.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ojbrcmva.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2beumqnop.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xbsuwluh.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2fqzmnrph.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2suhmpybu.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2labqeijs.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2thxkmiij.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2jydcymzi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2rieriefi.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2xhcklhdt.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2rndpjvsr.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2utubidyf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2dsbcshgf.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2qictuuut.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2bkmvwvds.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2sjrzleik.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2hqlduazm.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2udsjgrto.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2qdrhumgo.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2rfvttxth.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2rcergxpo.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2veqwgcuu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2cgwjjeiq.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2crfisglb.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2npbkjcoi.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2xpdneppn.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2ojxztohz.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2pcvpvkal.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2nzzhhvru.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2wrkmkjbg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2dmsaevjw.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2jzlkyfzt.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2hxigzmjy.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2jsaxspjr.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2getodnqb.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2xsaroblr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2hxbcglmc.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2rpsmaksa.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2cmwbiuyg.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2ydiwzqcy.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2cdoslaru.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2cpqxrdpt.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2mygumoto.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2zzbrquvy.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2hugcipes.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2sssntifx.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2eabjonpb.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2eczucstb.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2wfbmosqf.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2ixkbquri.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2budkbqne.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2zjqcsvbd.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2xzvwnxig.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2bzpruuxq.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ezlykbnt.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2unezqzdk.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2neqfrfyd.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2ejzdaxoe.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ofnaqgwk.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2mbshpkfu.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2gqbjvjca.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2mahnyqem.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2glgzyufl.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2lmqwadyt.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2ftqniksp.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2hwnjbqxn.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2adpjhpon.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2dqfwsvsj.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2cdzvdcrk.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2kapojdqh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2ykcfhkyz.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2jqvgzgge.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pwjwxprk.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2wkzgwbsh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2idliygsf.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2snpsnkct.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2flravhoq.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2nmhcnafw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2nrgruadc.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2aspojkvw.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2sliyjbmq.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2rxzcczgw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2xibmubqq.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2aogwqvbu.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2svytewmb.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2kivdkbpj.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2yswwehas.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2egcybnvw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2hunauevm.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2suocycuc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2nmaccuyk.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2soaexgwz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2tzenuoox.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2wnbgbjnq.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2uwpwyhmi.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2vkivzvse.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2eftvlkck.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2nkymstst.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2mpwruywn.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2khfvtovo.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2mobjjmhx.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2cmaokuyz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2azyixfvb.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2spmfhedt.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2tsqhzlql.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2jphdyblm.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2rlubnmqw.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2aifqrqoi.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wafoboqf.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2iosufgti.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2tjdfhiwp.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2rfupmzaa.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2ubevmfwy.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2fhvmfngo.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2iqkkbrem.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2ygsipzdb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2gwnqdmgk.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2wotrcttw.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2yhyyutfl.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2jhrltjmf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fnpaiwsj.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2njpsgtye.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2sggwgghf.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2atqzcukh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ldoymrbx.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2itosyqgg.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2vofbvkwv.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2rbzfdbbf.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2nnbagcgq.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2ssxbncai.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2xcvikbnt.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2rvfkpqog.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2fwmozcob.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dspsozqh.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2xanconrz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kwquqatg.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qnrclkwb.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2tubhigzh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2zqjlgmxv.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2yffpwpim.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2ulkalcgx.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2oismsjta.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2psqaehmd.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2ijvgaujn.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2yfjmdnhw.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2pnqzjpcf.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2sgyswcoc.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2hzlujzvk.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2micyucro.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2rrzsanjz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2jgktyksy.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2cofoatyh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2nkkjbsjv.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2hgiegmlu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2tstpacli.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2jopdxtli.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2xjrpanzt.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2xanyrohs.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2wiyoligr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2ltyotged.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2gszdbbut.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2yylaxypp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ycgythvu.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2biurcbnd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2ppuclzed.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2jvbdnjtz.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2cwbyqofy.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2qqigmgrj.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2prhgbomo.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2akfcuxsr.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2miwtzmcx.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2elumtnfn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2ohkfbphr.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2aickiorf.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2rdobgpse.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2qgjcrxdc.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2bkxqpkhw.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2jaxjfkft.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2csvjethm.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2gvabseci.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2osarhniw.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2xdmgpesz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2jbzwcifj.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2nfjdjpgo.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2emlvtkic.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2vtlciuqp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2qtjftuyx.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2azoiecya.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2qfeowjon.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2mqekjjqs.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2ussttowe.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2wxhpjwrw.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qvviqluk.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2gumlrirr.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2xikqszpu.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2foqjedvx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2ezemtsgk.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2sprwomev.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2azgfwfhe.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2bpuzabrm.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2pufzomvn.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2uszylzkz.html


<!-- 参考信息 -->