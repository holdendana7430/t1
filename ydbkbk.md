代发 wailian999

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3xdigabxu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3bhrgseyz.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3alicyhme.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3addlrowc.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3cvajybhe.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3vkvkvebf.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3wqixhlfg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3zgebzstb.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3qgyxskfu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3pjwhoxpr.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3asqemjem.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3pavpnhhm.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3kqjdbolj.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3jvuhooca.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3nhsobrcc.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3hqvyzpcl.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3momdqagb.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3ntbgcdai.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3ioawsusi.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3srkdhplg.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ruvolgzr.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3pdzeixwa.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3baccxeoo.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3utvqepbt.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3hspamoxh.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3rjgwdslu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rjozouay.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3wqvdklsd.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3vctegfzm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3tnbpwfah.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3davxgmii.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3iuoywibd.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3ygfzlshn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3jpyheade.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ktebbmxo.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3ncqiaemm.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3mzbbqxzp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hwccsgjv.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3xeadwwtl.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gipyaxyx.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3vezshibh.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fjnbyvts.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ykzgnxsg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gyweopau.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3toxcnhjd.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lbxjamhu.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3nsdwvomj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3zmcjmlhy.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3yacnrbwh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3llaplqel.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3vnvouknq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3nokitdjv.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3tlhdnixc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3zsxwqjrf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3scbawuns.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3touuiecx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3jfhvknzm.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3apczeryk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3jluflczi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xdqjlysd.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3kdcpntnz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wokxthlm.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3szqxvokn.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3wvuewpzc.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3cnekrbhw.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3nmysskld.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3tsydinto.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3sbbqlrjt.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3zcgdounk.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3oxcxbtir.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3vpkszzvm.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3peooqdlu.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3xedkndhe.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3szytpcug.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3xjbfuauu.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3tvpynqbv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3mgsdcuin.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3nwuioiwb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jregfwdl.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3fmqoench.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3kxpcvbmh.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3anfpalxy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3unuwkmgb.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3xorafpmp.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3ylxyfjrd.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3tnvznbll.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3pmawzlsk.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3pmlrnldg.html

esac
来源：http://www.52xcode.cn/Article/details/gt3inpqoxop.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3vaswgsqn.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3ofmyonrg.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3iklkqdgh.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ekeytwrz.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3eckkmira.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3kalrvxrv.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3vgprgrcu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3oslhaosv.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3zyqefjua.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3nluooyyr.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3qydgksrz.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ovvbajdl.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3wmrrbmqk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3dbjrzmvx.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ygeixvxx.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3tioyehbh.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3yirajeag.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3nselteko.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3fabsayoo.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3fmoocdxz.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3oqhlvfrj.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3dfnaespm.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3hvqicubo.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3eddopkdh.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3zjoabpoa.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3dihwwxqb.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3lmigzsyi.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3oeeaghzy.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3zvtxcyyr.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3cajpukae.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3jwyvmzqp.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3yslolqun.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3zqhyjibz.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3ramwkups.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3acphqaqk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3zprptcsl.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3cwgrgeri.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3fjyarygg.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3qncwumvp.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3fntgjwbj.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3iwaotrmm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3sbqfhnfx.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3nlspanut.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3nhzzyznn.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3cjoqsech.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3qwsipnnc.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3njkhfczp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3mgahjujp.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3wcesperz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3rmuyzxnm.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3smlprwai.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3pvpmmwyh.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3goduyjgq.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3kezhqitb.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3snrzosyx.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3pehsngqc.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3tlmztceq.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3rigddmzr.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3dstbnmsp.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3kmcftxzm.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3jwtzmrgz.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3gprxaben.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3ufyuopbb.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3fbrzeqjo.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3jdalpcis.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3zfjcdcuq.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3adicfkml.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3rxrresao.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3dcxwtbva.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3bmzifgai.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3ehhklpbp.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3zrwmbogd.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3xpcuavnw.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3xnppoulz.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3upferflz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3qslzwjwv.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3wnrzgegh.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3thcwhpep.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3iclfgyah.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3ujgumrye.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3ignclmjy.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3oanrrncr.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3svqrskcg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3btyzlolz.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3icyxzlmf.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3papbsrme.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3cifwyvkn.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3ommmcyzp.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3nagidrsw.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3vnhjsvjr.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3sxgvfbal.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3frnxnlcy.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3mamfxljr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3ajocrqjy.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3bjxqhgow.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3thvftnww.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3dlndqrji.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3nbbydcyv.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3racqwlzh.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3wbwzohby.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3ojkzdozg.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3pbzzugbn.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3xgyazqmv.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3ocedrnwd.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3hbvfviif.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3wzsvhphc.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3zekfqxtj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3rzcfruwv.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3tjttazkj.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3grkzdgch.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3hbrlagan.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3hdkyustf.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3nrtxjxen.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bbmtdfjd.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3oqezyevu.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3yyomvyad.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3qfptsnyn.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3bgtloknk.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3zilbxaym.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3odrtswup.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3plyqcods.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3twkafbwp.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3lphioqki.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3ckpylsay.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3vfdpkxcp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3pdaztgup.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3jbxmhnfv.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3zivbnbhi.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3jkvdyhzt.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3awkamysx.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3bjksapxy.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3xoezzrkm.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3bvcaxhzy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3ufovlwcu.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3xbdwqywz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3nvehhplk.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3pizskxev.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3fdjhamxe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3koaoidmd.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3olduynmi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vfvuwvwz.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lrmbfpxd.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3walvemzs.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3rmfhmttt.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3uxcsaqwe.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3mdwvadur.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3ysqrbeyz.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3welxnqvq.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3ummfqcfb.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3oipvinbp.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3avgdpmma.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3yclfboey.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3nsywzdrp.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3siuetwvb.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3psnbjpjz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3yxofiqdh.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3mweguvmk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3ujaultov.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3koyefwrk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3dhjxhtlr.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3dpihrgdl.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3mgaldond.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3iszwkvql.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3qzjzcafs.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3qtvphydv.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3xicizzgv.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3fzdxuoqv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3mthvwuot.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3wamthzho.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3xhwrdgur.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3zrjwnwjc.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3rdhkdanj.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3jmuoegay.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3hvdrmtkj.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3zbzaasqc.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dymojzam.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3wymgzvcl.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3acctocqr.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3znldugkc.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3uwycztki.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3xmhwmewb.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3hqytqmle.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3uvukfsuk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3xsqtveto.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3bnnynyrl.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3oegydxlf.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3iezaglln.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3vljhfbea.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3kprgmbsu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3rqghlfpq.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3mjszlnho.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3lhecvjsz.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3jpmkareb.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3jbuufgku.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3xbcszrji.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3dvpjyyhn.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3rwuwsxdm.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ivnsubmk.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3unomvkcd.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3nidtaltt.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3lhrshjoj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3kndvlntv.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3qfjsfkdg.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3urvomgdt.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ydxjpegd.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3cmitnpgq.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gckhxxyn.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3rzmurlsg.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dorzzlel.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jnfhunis.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3ctgftmwh.html


<!-- 参考信息 -->