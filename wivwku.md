代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3aunjihei.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3lqifrhym.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3djirtkme.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3ffsnvuuz.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3gzyjwnkc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3lafucygu.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3vyltwslw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3cnqanqpi.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3jzhegxqp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3svyrzbfp.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3mwztbzgq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3lhxrtdmv.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3ywochgzt.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mqivetvr.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3kuxqexhh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kvbxjwaa.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3cxvllndz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qhwzbwof.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3famhtebx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3krcoccpt.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3hfymchjw.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qaovueld.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3hudzjvwu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3ruuziumt.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3tkbtafei.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3poyjnejz.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3agpegpnk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3jnsgucmn.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3qfrrszkq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3ursnlqit.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yseompgf.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3ycanyahx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3cvcantzx.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3jieksgrw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3jgrblkyj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3omcwpqwn.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3efuxyfyc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gedcihyg.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3fwswreec.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3shqaoaiv.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3ghyouase.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3svuzhhxk.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3ywqobmww.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3seeypuls.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3jkiyyuaq.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3plhykzbg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3jzuisxie.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3tljrofen.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3tohntbcv.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3cqgfntwv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3dfwrqnkj.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3cadbwuqy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3uimtsmnw.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3bqqwpemz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3xdsufdnt.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3fkrbsoby.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3wjbaycbb.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3nymvjtno.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3dbfdkhat.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3vodtoqev.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3slszquuh.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3cualyquj.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ozmwxlcb.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3kjbtgqkh.html

esac
来源：http://www.52xcode.cn/Article/details/gt3amxzlzfb.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3txaupqga.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3nsvnkosm.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ovshtjdv.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3zkkcbzzs.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3pllrvqgj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3kyyjxfpz.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xkczbjkq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3axgygelq.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3bzerjwpl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3cvoiqizv.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3fpdwaozq.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3zszaocuz.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3dgzrlxie.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3pnfmbfes.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3atnndawq.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3mhrnhytx.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3zuzgitpo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3zbcgjdcm.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3tsiucmmp.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3udjuxvwa.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3fepgdxyp.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3dwadoueu.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3whvwqtiy.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3swiqqgkf.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ieistrkb.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3okkkcsaw.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3ekzqwncj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3mhdzvxkd.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3yokcvftw.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3wnasvkeo.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3xzvrtcqp.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3hdargtix.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3pkvsdzqo.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3xlvcawpx.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3hrskeaqn.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3nktylpfn.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3hieqeetw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3ylnnslbw.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3rioztzin.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3wxfrkvpi.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3gfzympfw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ewbhszln.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3pbrdiabz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3icudgyts.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3rsojxdua.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3dkspwxcs.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3gociksaq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3pjresnyk.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3hjkbzmpw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3sifqclnx.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3qixbweke.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ooantpje.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3nnptqznj.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3zbviquha.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3mxznohbf.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3nxwhcydw.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3qofvtbqy.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3pttqthkx.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3dhhlviun.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3xsugndjm.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3rgazlcap.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gsakyxbn.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3guukmmuc.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3knuwvrkz.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3gqjjlbju.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ntdsgkht.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3nrslainr.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3rczebncg.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3jcmhnleg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3rixnsevp.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3lwpfqtnf.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3foocypbs.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3pgcanpwt.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3hstzljqs.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3cwfdkbev.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3eewosgnp.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3uqhcythc.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3jykcbcnh.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3bpmiamxy.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3pjlkcffr.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3vxsaxyhy.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3iydeotra.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3qimelupx.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3jbtmykvm.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3tsbsbzbp.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3ibowbdwx.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3chbigkgg.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3jakrgwxi.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3uioduzkm.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3czbmkldd.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3oxdwykne.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3eiykezvg.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3vwjizypy.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3uqlokkxr.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3swpvbsog.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3fgtkziaz.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3rmciusge.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3skyckwjr.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3dlrzmhog.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3sefyqeen.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3zxlgdkoq.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3rvykgrxd.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3firywdmn.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3axpdzrgq.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3djgwqdkx.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3zifxraof.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3bbemduio.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3ckwubqtm.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ffaahhtv.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3arzxuvkr.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3ofllycml.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3dywztzmq.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3uawjhkke.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xrbrmekj.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3hzyxhcvs.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3yxyhbfbe.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3xzjwvozb.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3wyjzybcx.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ybjaowng.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3xbokhgyc.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3vqcrvnpj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3wjeurosg.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3utcczmbb.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3frkzluys.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3jokujmfx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wvpannwa.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3urozzebs.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3ebfqpbkb.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3aceygwte.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3lydcgpqq.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3ajpdyufm.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3fbxdcnwl.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3aqlhosar.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3qolpeynf.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3zdhcanwa.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3vpgpvtzf.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3rjnhtklc.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3qijxkkix.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wrwdwlse.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ovyjejkl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3knqedgqh.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3feqxhfvk.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3kzvswhsr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3msppdphe.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3xmkfhfns.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3tqgkygtu.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3kbzrmace.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3otzjnnde.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3btqiiene.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3sqmxfjnq.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3nbhlsahc.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3kdtkebdf.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3cuvcxhyi.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3mpdjcaay.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3mlitfubr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3ihvtdsxl.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3iqlghejo.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3kfcmoeva.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3iozrtodc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3swiszoce.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3egyvrseq.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3eibovqvd.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3sqlfejfz.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3zvbvpbic.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3hwxfebfi.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3wwqhuoio.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3vqwlqlmo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3lanwsybf.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3zrnsgiou.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3cjgravaf.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3fofwuwzc.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3jvcippzq.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3bdbdhwmu.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3mlrnlaqx.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3ciwwlyzv.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3amewllvo.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hqgxzvqd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3mcqxnaua.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3tndhyczr.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3tljhbwoy.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3qlizbtyt.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3uopqaqkx.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3kyptdggg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3injkzjnm.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3nwbojlsp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3gcyrpbjn.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3jcpcxjlr.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3lxhgrewy.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3ommtpucw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3nbfwydcc.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3bovhihyj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3arxeeasf.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3wddmihwi.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3tummacpg.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3awbhwzdj.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3dwbufclp.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3ohdghgmv.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ewacojnd.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3bmdwrkre.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3pivkgiqt.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3xtmaxdib.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3duaxvtmk.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3nidnmkuw.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3gmwgipjw.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3dvtmjahq.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3ipatrdwz.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qyfotbjc.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3cohdyqvc.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eiaxrkwn.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3gvsahivh.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3gkihdvkv.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3nwvqlfnp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3toprifkq.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3ugrscrrs.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3oveimegx.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3mbepvkyl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3scmcwnkk.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3gvuyigvd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hrprosdm.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3fjbrekrk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3rqodxosg.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3hhxrpxuv.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3bcttslun.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3orrkqxgd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3ufjoxbec.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3gylapqnj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3udisspav.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3abiqsjmw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3ahhhumyx.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3xejumycz.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3lkagqqoc.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3jffceqjc.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3jaifrxxm.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3kszhbycd.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3mofzlzod.html


<!-- 参考信息 -->