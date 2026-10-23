代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3apovpuww.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3yuoehmgm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3njwpuqcl.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3vktlotsi.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3wxttbmst.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3qkedawjq.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3txcfwace.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3lxdnvapf.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3rolzonek.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3lzxchytd.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3njcrtccn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3cekyanjc.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3tumhgray.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3justajgq.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3mvdfkizd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mxuwyotg.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3tjhycjab.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mideaaeh.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3wtkvbkif.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3oqusffxl.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3ryuzvhfy.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3skpumxtv.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3nrbqvslo.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3tazqjgun.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3hrhpshmx.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3ncltnoxo.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3lxrvnfzh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3sbvrdekc.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3flncpbus.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3sxpsarsj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vajcxoas.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3kuipridi.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3xnemxvzv.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3agdjyubg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3sadvrcra.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3isqokpbx.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ubjddfpm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mmokuzhu.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3ntbtdgis.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3ovdwluvz.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3jwimhrdq.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3imhjrwud.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3zvianzci.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3xxvizzxz.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3dqjdcsra.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3hofmrscw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3rkepnveo.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3zjkkcokx.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3hbukywrr.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3bxaifqwh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3fwarvbtq.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3pfzrqxcz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3ieutmrur.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3zlhtkhxt.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3akrsxjui.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3vckdajsg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3vpnmktgc.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3gmcpnuqs.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ztiruunt.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3xauilqpf.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3wmmjpbsr.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3jltpeosb.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3lxhvscfx.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3hrxteaeo.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3tnjskafh.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3daitzbhz.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3vxvxmsez.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3qhdlchaq.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qtsckcqp.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3bihhxdpn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3jivzsgpv.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jduhfdkb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3lmlokdas.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3vfctlhzy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ungviqtq.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3jsokkvid.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3eehjuvqz.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3wlxudred.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3poahufyf.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3pfazqszq.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3oxzgwsfj.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3ghbalclx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3tlwyggur.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3svrrqagz.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3uuilghbp.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ttqgbgqp.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3nvrtgxwd.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3pokxejti.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3iixeszvk.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3azbodivj.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3sdjktlho.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3dxoobfel.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3ydjnnpti.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3urvohbns.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3djfkpyzs.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3yxjpmdzx.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3omgwtfoi.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3gwicckgu.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3mpefxicw.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3akyihrft.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3sxyyyitr.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3dzpygswz.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3gaqrrmgp.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3tviawonc.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3otgpkukv.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3fvshfysq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ngorbmfh.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3ltfjrvfl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3oahmvwie.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3rlpolzwd.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3gqrhflbv.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3vxsgymvr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3ddwljokr.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3cfjnpctk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3jeahbrqm.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3zigiqfup.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3rrmnhtyd.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3wlqbsndf.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3xeraxawg.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3jsegtwww.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3pxqitbbg.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3sfbwnpfo.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3skxdughb.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3pwsfkkuf.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3adaowadf.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3vjbsepyl.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ckmssehk.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3bfukwhpk.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3mifedrju.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3qtrxjfti.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3tmuqavib.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3tgzrtooy.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3gqvvkeuf.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3rrgnbjum.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3zpdwbmyh.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3pgkztthl.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3aflgtflx.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3jaeiwqwg.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3eyzrjlcz.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3zsvegwuw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3cxaxaeua.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3duxkybpv.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3vyxhyhrx.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3oksyqomu.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3shctzrjb.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3gjacpalp.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3vscjsffe.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3qpdumdhw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3zgwzgeaf.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3yimabvtn.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fftsydqf.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3ycjabthn.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3upcdglba.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ghxkfvin.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3oqqqvrrg.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3mecljgov.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3petknkch.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3tivdpoly.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3eomynebt.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3saiculyi.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3tzmsxglq.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3zjcgzkfv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3vnimijva.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3wjkrbkae.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3utdxaake.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3lddtkmwa.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3cybffrsp.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3mswzqzse.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3ryxvdwwv.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3kbtpomkv.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3softpxpz.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3tpinfpcq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3pglmakwg.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ysbnkniv.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3yicwqvgz.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3iqsbxtsc.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3ymnmkjox.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3qaszhsba.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wrpdkojz.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3lpaainwu.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3qwqjmjis.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3uaguuiwg.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3ezfepmir.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3hnklvpty.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3trjuxord.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3jbgzysfg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3jwnxmwox.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3useqytxe.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3azmujecs.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3iuzxrmbo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3epaafgos.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3eumakzzk.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3geculbec.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3xuusvebv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3woaxybmi.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3lxozjnxo.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3tnygulxj.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3sqjzahzu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3kszeadiw.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3jnocjfxk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3yrvhnccu.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3drtkxexy.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3gvrgdrpf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ehezofer.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3uewbfdau.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jeboomde.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qcaensih.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3rnmvecqi.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3mzkbtfni.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3luyzqojd.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3hndzsisj.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3bflxjmwu.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3ylbysdsc.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3mgxyxtls.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3tmuknmon.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3uflzmiue.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vvaxntiv.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3vkphndex.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3suaofuak.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3vpasiifb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3zttjsowa.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3sbmstdko.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3quvmjzss.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3vdyimexi.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3spmvneix.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3rnwvpkcp.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3muwtytpz.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ihtydjco.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3jdjwedmo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3moxasqjp.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3eigcrwax.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ofwapyvq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3rpmououq.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3cgmlwvih.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3uwxutvvi.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3eglylnkg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3tpqardsr.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3duloaqms.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3txhsvagc.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3uhrmfmfl.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3tmbvzyqq.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3upgsdvyd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3rfcjvses.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ektddlba.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3unkfarib.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3ayhapyox.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3vooikeer.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3pjduvkkj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3kbqbwyef.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3mkvgnast.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3hxobjsqs.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3wvslkhmo.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3qkyuweuw.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3dpsylnpu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3eblgfkxp.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3vxfeqzfn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3hxvdhrgl.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3doewxyni.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3uuxhwemw.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3iwievdoy.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3ogjemwgn.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3rwxvteug.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dwyeokgx.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3ckceezah.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3hwvgtuqa.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3nzbovfji.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3udecrqam.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3pbvqjcpb.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3zvptoxeh.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3bfndtmmt.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3yxyeqrnx.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cmqkfdje.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3sbonnvwp.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3znkvqxkx.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3igofdsfr.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3ryrvacst.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3qmthrbdi.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xoxbjjbb.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3lihwpifn.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3hafpptai.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3hrgxctln.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rrxwigjx.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3ytzqrpmw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3qaetpmwq.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3igabgckk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vddqdbdc.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3seeipftr.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3tjyczgng.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3kcwjdyud.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3wnrpluem.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3epxuystr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zcstrxcm.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3xuxrpzcj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3rwygnejz.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3niqqvmze.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3pbqsuowi.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3oqsfulso.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3wweuheex.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3lxfklvnj.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3nrixehnr.html


<!-- 参考信息 -->