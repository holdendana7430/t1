代发 wailian999

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3jzymxogu.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3xiiwbzjj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3mqlnjkhr.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3hrjwtrba.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ndxjcssx.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3kcoutnuz.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3etshhjzj.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3ungckgkj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3rsaftmlx.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3pxfaxhog.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ufhjrgvo.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3cktochzf.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3hhdfalqy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3parxggzu.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3wfrcroao.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3xhmbcwia.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3jkqipnmh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3jwgnawzj.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3rvclwpgs.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3htpjulvd.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3mpwvplok.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hsseypjl.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ckayxwuy.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fosmacln.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3vuqanybr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wnahsmli.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3gcolkrov.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3aluyphha.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3rsiwjeri.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3neqoeksg.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3fwlmekzi.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3dfsyyomf.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3ctgcbowg.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3merfxwtm.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3guuvvhho.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3typfwqdi.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3jogjrmql.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3rabparzv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lxbtzukw.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3amxizdrm.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3qqymhzez.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3oxloqkbe.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3hfwbeekz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uijbfwsx.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3vznsecek.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rosroxkn.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3vxhengdp.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3vmljjszx.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3hhvsmnev.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3axbgfqko.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3mfvybelq.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3ngkqjesl.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3ebxlqtlt.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3bskgbobc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3bnjcmgur.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3fdlptzxb.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3fdyvqvsb.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3recxfxhi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3qgxotpyc.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3lzxzfduo.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3nxcidmla.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3fyfpwkmw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3djhnhaqv.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3eupeqqxg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3alweuela.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3uijkbyvw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3rhcjjoei.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3ubweppnd.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3abmgxwxc.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3lobwfsaq.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3emhajpro.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3gfpqqqie.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3hcjvicjd.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3jbqrsrkm.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3kxhydbrw.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3rkymqvcv.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3kgdxaktm.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3sybhchbt.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ldkesafv.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3pgqpwmxs.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yhunvllh.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3hnsssmyy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3gxanpwbl.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3gdchfafh.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3rmlocxlv.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3cozbwegr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3engenbzh.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3djmeeyzj.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3qwachwkt.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3nlaaatqn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3kfzlayou.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3kvjhrkxv.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3jcnqiyfc.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3nsykqhyq.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3oekschtz.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3bezaxuwt.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3patgyods.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3hdlhrnhg.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3tzaynakk.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3jissxewz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3jcpbyqpe.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3pnybzics.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3uvsouenh.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3bpbgypmt.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3mlljhczm.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3drzpsmil.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3rkmkextt.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3scgpbgti.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3demftfyr.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3ccyfyhar.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3gxfcfljp.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3frlqkrct.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3hxhphqcr.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3fazticdn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3wybwnvnw.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3hbuskakw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3blcrgqtb.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3enaajhod.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3carfacvp.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3ucdarhpk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3zedqtocq.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3ttotfbcz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3wjadnkou.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3pbuyqlzf.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3szvwcgrt.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3tayofuea.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3bllzuyds.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3bmihejyx.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3wquimvsj.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3wkibpetf.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3aytxyzlr.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3wntlxluj.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3hyltsyxc.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3szoldtmw.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qvtrltek.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3fkxjbhbp.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3teorfrxc.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3umflsvns.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3prvztcme.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3rbolupab.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3zxvkjxkb.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3pkaurnqr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3wwehzudh.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3iwsarkib.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nxseoorz.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3rwrcltad.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3eywfvxjs.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3egzmtuvk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3ayhsfhub.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3okzgufyf.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uqzqbwsc.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3xtialdcn.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3cjvyseir.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3feurjhfi.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cnnmbryv.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3zmbpruus.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3vypgsush.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3gyuwjrwg.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3qflkdbgr.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3qbqaramv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3xrwbkdpu.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3hdwrhdog.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3gtzpxskh.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3vewiyufe.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3qnigvbnz.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3xsakrvwj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3iirjodii.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3zmbmsvmw.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3ruxvakyw.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3xitrjauk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3lqnfhdoa.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3wnpyhwzo.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3winxygyu.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3wfphgylr.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3kdqpombd.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3kmrbxexo.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3xglmaqyr.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3judxnhxi.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3yingypxr.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3ihstyhyr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3tieitajg.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3rmaoeunt.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3ciukzuua.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3kfobvpej.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3psqmibfl.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3oumyetqx.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zwnhabml.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3ehgsjesw.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3hryyquty.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3pxggpymg.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3dukmszso.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ipgeivye.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3eunmnuqm.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3qcwswzjk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3kkbeycns.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3rcuzegsd.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3xwoxpjsw.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3ttteoloo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3tufbwavb.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3sfsdkebs.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3pnzunqzm.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3gejkcrsh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3roijgdhf.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3kifudjmn.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3jpsaicrp.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3yxmjouin.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3dtgliwld.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3ylneuixp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3sptgcgjt.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3ocyfmmli.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3sxixrydm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lekykqdu.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ttrzoden.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uyghxtgx.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3oxczpkms.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3aerijxsa.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3nadzycqo.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3fosopbml.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3szfisyff.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3kkgkyevq.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3ifkfvwbf.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3nywrbkwy.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ndxgsmdm.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3hzxvyemm.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eeckrdov.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ffceuyma.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3mmxedwqr.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3yhvpiqhy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3tdjumdrn.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3xtqqiudl.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3mqfgoocv.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3jrrrlozf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3xfeljmsk.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3milebbzd.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3xicnkule.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3meuzcrjj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3esrxalvl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3uefciikj.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3hhcskitm.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3baenaiye.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ikiztugz.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3znlizpwl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3faqphwnl.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3pxhcknrg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3dnaczzon.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3mndoebjm.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3xhsfztzh.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3nverpqrw.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rwdmxywh.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pjsxvbag.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3kvezppno.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ikkbldxo.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3bwrlyyec.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3gjwuxvjn.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ztinphub.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3rytbkdva.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3hdummtfs.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3kalelffv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3jygkpxcs.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3dbgpdtop.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3zehzlpai.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3mfcfwcro.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3saqgotzy.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3cndsgutz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3nadhqohh.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ynpbzcif.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3uoaumlnv.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3ciykbrzf.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3wltfpfej.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3khtoplim.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dhsrwnmd.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3lcshhmvg.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3megnorka.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3pzjrsbjv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3pdjnucdr.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3ikxcccds.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3emjllarw.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3jgnodhyk.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3nurnbsuy.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3soicbtid.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3wgcndtfg.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wmovpuie.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3otsslqdv.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3vudxzckg.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3yhrirslc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3zfradcii.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3jmfhfebv.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3hadtscfj.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3zbboahge.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3kaddkkbr.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3ynufncmy.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3csbdfjbr.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3avxailfi.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3uvnsycmi.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3yzuuodqp.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3arbyldel.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3pgtfxjxj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3lurzttpe.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3axixepha.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3ppxnbefn.html


<!-- 参考信息 -->