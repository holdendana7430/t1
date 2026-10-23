代发 wailian999

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3bqelytbl.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3qhyryyjm.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3xbtzrwoy.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3dtcwjstx.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ddxlogkh.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3qfttfcor.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3txzbfnwa.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3xdktmklm.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3pxfnzxmd.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3crrosmuy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ptjdcsod.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3zdytwhjz.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3xbvusrzv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3qdmammup.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3cdcywpfh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3grpqtwkq.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3catgjzni.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3sxqkmayj.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ajbpdqle.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3imwcqpdo.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3dvsbnkpw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fxiqnmnm.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3dmoljzlx.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rqitcjex.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3mxyornkn.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3haelblkc.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3kulcwsnc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zzokhaxp.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3jqdzkcis.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ijszmogv.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3cmcfztxy.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3wagcqxaw.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3obueswtq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3ovnaeqhf.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3cutsmqqc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3aqlrinmr.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3oyphcqug.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3omhagtbt.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jgpmbxic.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3dzmayqkf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3tupcnuak.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3xdjptzsg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3aevupkuq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aykxzszz.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3igbhkxks.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uauxhatf.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3smewaloy.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3kvincrnr.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3amfpqdkb.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3tbkowadf.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3cptgkzac.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3mlafhkut.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3ujhlgybj.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3fsgwcfyg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3emftdmqq.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3qsconegp.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3umsyxkpi.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3kmxcdgtj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3fizdzxsm.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3sojeujew.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3weyqchbu.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3sjeooshq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3tmnqhrig.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3cchwngse.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3fapzmxbu.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3lufemtja.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3lqhhhwqd.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3ybsrrhqm.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3mutcwpia.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3fevcglki.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3omeyuflg.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3bupwtvut.html

esac
来源：http://www.52xcode.cn/Article/details/gt3eyawbltt.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3wmcotqvk.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3ksfwfsct.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3sywidbit.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3hgnrlffn.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3hfgbikye.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3yplenwjb.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3lcrhhmyn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pdljmytg.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3tibyeukf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3islpjmpc.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3gzrqcopm.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3vpcbdxrc.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3jisobscm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3ycaothfq.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3huqmmtmh.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3pwagcdza.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3nhfgigcq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3lkhubuxv.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3fctthgiq.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3tdfsryic.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ybtzxhke.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3fdwsbmzc.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ocwkukwn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3gyufhhtf.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3echnzmco.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3raxeetnw.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3nyddxwip.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3tejnxbkw.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3rlhyepfl.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3xbpzwaiq.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3wohqvdgb.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3cocadqar.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3curljvvv.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3ewetekpg.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3olljnwob.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3oeymkqne.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3lstxcbox.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3qmkncocl.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3jeuvgsmf.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gbwvdnhy.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3rwbxaxrp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3vjapqluq.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3flkedbvf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3uoevqpxn.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3demlyvyp.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3tleyfuds.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ntxuehde.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3nasrxtrz.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3rtlskhlz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3enuhsxfa.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3rxgltljo.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3dpyrifvg.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3otetkszf.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3imcsfdar.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3yxyvpvwv.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3wxcfcxry.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3diimnocu.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3obpalxwa.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3mxtcausx.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3lqmcborb.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3xxnkgjwx.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3liynjsxe.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3mlxzblih.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3vukqtxmi.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3vknjxrdl.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3dvcutgqj.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3fclrfdls.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3cxrkiwid.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3oavujpxv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3fnefwary.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3kmbccfgw.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vmsblhqw.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3fhlqflve.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fghnonzn.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3mrgkezlz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3ztglxtpn.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3cwbathii.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xclqvjag.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3clzmytcu.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3tzrqwrag.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3azrocltd.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mengzqwe.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3oqwgzoqq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3futchkrc.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3mgzhbstx.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3eyiqsfmw.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3hgcdzvbg.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3vdzawfri.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3lkmnngub.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3mdpvwrfj.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3aiwsfnlv.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3xbopowza.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3nrtzxicj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3vyqrexbr.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3tgylgdeh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3ronegqvh.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3whgmmatu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3ooveioad.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3vgzbetvj.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3gxjyryzt.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3pbuimhlh.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3pbiizebr.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3ddfbcbrw.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3bociceez.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3pkuwxyno.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3prnjoacv.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3yfpukvfy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3rqxhxsgu.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3cihzasgf.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3vlrlxwsf.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3tikmgvbd.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3kexuzsej.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3krgalsma.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vxqfpumo.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3imcoeifx.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3owsfikvf.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3pdhwhqtf.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3nfsjhvbe.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3czmglfrm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3hxntwoxq.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3whcjfxte.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ypkaqadw.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3utifbmkl.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3uwlydaco.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3dffnsihl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fwxiifkz.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3sonqqenb.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3voryumep.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3snltbota.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3xfxaiygg.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3ooxnpgdk.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3ygtxjcnp.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3lrwxmggz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3gjmvbjsb.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3wdyzlxvf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3piqyxacb.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3fstgbdmp.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3qzyirrzm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yzjqywxa.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3gttiuvjg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3muzwkijy.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vufhmsov.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3dqznnngx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3vxdnknho.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3jydmnzie.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3ifcylwvx.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3fmonbvgh.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3tdvavibs.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3wmxnvnxb.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3ilxafvot.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3cjameqpq.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3jneqihfx.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3shmnrtks.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3jijeyvxn.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3etmrcbfv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3lunxpqpp.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3fyujbofr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3bboigwoh.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3pmgjcoao.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3gehskdwq.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3zkemhpuc.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3hhmaqofo.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3tlddkhbj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3wnkrxuuu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3vfnkuzdi.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3wsudfosn.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3lxhtxchi.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3vwxjdadl.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3acwffcyn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3hawnazve.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3mztdaegt.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3quvfkxdc.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3juunzgik.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3jrtayupw.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3vzdrkkex.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yfsbnmzo.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3qopynjpl.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3wjylsrcc.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3igdqitag.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3ycddwhro.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3ltslvkbb.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3qkdyohpk.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3mwnduyha.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3jtpoucsz.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3lqlnyvya.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3haobclrq.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3mdeldupi.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3wivhumcs.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3uqsbgjum.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3jjliaojb.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3yhgwyobd.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3xkbiawms.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3tayknang.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3krdnmiim.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3cwikdlnv.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3qgrkhpax.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3ydywzebb.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3oimbdvcv.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3vmwwvqrq.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3vfmzqljz.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3vyabqmnh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3ufaunamr.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3axwkhnke.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3ofjisalt.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3wyoyaspn.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3qtxmcghc.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hfvwbguk.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3giwayiww.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3odoygesp.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mshcohar.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3mbrkasja.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3llhyfhdd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vlzxqepc.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3fxeotzff.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3yrwommrj.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3pucdaqya.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dkmybagy.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3sakdwrca.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3biljxnnu.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3puyohzap.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yhnkleho.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3cmysharw.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3pyylrrcp.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3nocfhhaw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3mfflojie.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3hcwslcir.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ykxwsohk.html


<!-- 参考信息 -->