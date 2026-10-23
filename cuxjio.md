代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3mbkvsjvj.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3qrumrsgs.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xrnhmvkf.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3ohsaeono.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3vvlytpzd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3wnoirbls.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3pceciguw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3xzkexuor.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3svpvyktg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3nftoiaug.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3zdwzlofo.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3izslxeso.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3rsyqxrlz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ihmlggha.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3xmvynybn.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hcxtintv.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3incqnqok.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wyafnwta.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3abqcmqka.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pmocgizc.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3ucdylzcw.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pgxpiiso.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3nxujlman.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3loefzgjr.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3xbysywtz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3voltbcyz.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3jqisjcml.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3wqdzpsen.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3dnavoklv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3upgvvdbl.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3caddbbop.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3felguivw.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3ahuvcrey.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3scniydpj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3iilawagr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3chrcopja.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3pjilrsei.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3poenwkpz.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3etmejfve.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3myocxjcv.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3gzeliwcx.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3qwrtocxr.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3hniyozse.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3ofrmdlsc.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3psnwmkfq.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3pvqgzeoz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3jkqveipm.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3uajginjm.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3qmdpecon.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3silmitxb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ysobsnsl.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3jiqusoly.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3vgkvakso.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3guyonaom.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3yxtfgfek.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3pijbhzjv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3evnukweh.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mrfjzumc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3uewwcsfj.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3etoavedu.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3fklhpegd.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3yheqsmfm.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3wextyekv.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3iefwepso.html

esac
来源：http://www.52xcode.cn/Article/details/gt3vwzjdfmq.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3gczklwrg.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3bmokfjau.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3pofqkaom.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fweluebp.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3popcgjxj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3nrtkaylw.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3foyvtjeu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tuqdxbph.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3xmwsofoj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3pvqbgihe.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3vxllpozq.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3vkldilpv.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3bayxgrpw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xqrsgfrz.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3qitzluct.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3icojmogh.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3hwhjivxp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3mfenbrtz.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3jncpgioh.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3umlbpvdm.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3gglchirr.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3skcdjjmt.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3nznkpdko.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3diyxrabu.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3hftoveno.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3nfzwnulr.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3wkjvazbk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3kvpbdifw.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3gkzeywds.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3htpkfyrg.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3mqfvwnon.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3wutvsrdr.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3iycuqzly.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3dvatufjd.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3yapkrgen.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3jphypwro.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3hcxugbsf.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3xmkhhcll.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3srphyucn.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3zonejaid.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3ukunoqxp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3utrzcren.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3bosauigs.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3wmjsrhec.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3hsucvcsx.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3frstupen.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3icbicwhg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3ohhuxzns.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3geozwtqv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3jdtcstvn.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3rmwdqxfq.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3gdgmifqf.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3ergfkzsf.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3uobthcrz.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3xstgsgvq.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3afkljcte.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3qwvxvzlo.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3atilpwwq.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3gfmplahe.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3dgfgjnxq.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3yqhrxqmp.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3bhjrsqub.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3aklnppod.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3buazoiti.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3ukrgozpf.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3jxaakgqz.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3texpmlpi.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3sgaqxkwz.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3mfyfckip.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3gcbdbinh.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3wooczpac.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kldgcxzt.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3trpgvlso.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3pfjptkpd.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3lpgxzmpn.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3uczrnowo.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3qtogehpn.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3bcwjvwfe.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3txkzvgka.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3aopicffm.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3uokrvqnx.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fippkayu.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3kwifhwpu.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3hnrdmfsd.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3ecyhktoy.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pgrvobbr.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3aykvaxxm.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3zlugvpor.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3qyrbrjkm.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3rpwlkpom.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3fhpjliyv.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3mrbkvzta.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3djatmaat.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3snjuoxwu.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3wsmqqsfz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3pdzseino.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3wrwdswzb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3myaduyia.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3sljqmaps.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3igjnxgry.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3exghqhcp.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3fjxkkztw.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3zfhypexr.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3niwyrtux.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3wjhravqy.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3fwmzsxga.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3yaehqimb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3kjrlcrzn.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3kyipthzx.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3howtdkzz.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3yxyflglg.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3apoxpweb.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3kyzxgkoj.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3wvfomhku.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3urlhdyms.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3rtvjtwqg.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3liukvefv.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3eunqxbfq.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3zcxytwqv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3tyuwxfbo.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3nhprkzkr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ieaehlrk.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3bqmcvagy.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3qnblwwnk.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3rgvogcfj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3bohhsfam.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3vecncemw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3tpthzqwr.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3ddobwnlm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3ejlxnncu.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3anmujbir.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3uxvqbvjr.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3qsayplvy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3mhbksrkx.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3oxxakfal.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3exsovppq.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3rbsvfnhb.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3lkdvojhh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tsoiehov.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3dgvkthic.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pzqatgij.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ocivrgtz.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3jhfqjxnn.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3ymeitrid.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3gpbzhwph.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3oelgzxbz.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3wuvxcpij.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3atkusmhy.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3bnhxtrbj.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3pbzypkfi.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3qtteagsz.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mfoudkpw.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3kvmzbnvt.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3enpnvxbg.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3jwaafwre.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3stnlgtcv.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3zubxfzzk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3kvffkspw.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3cdltdrwc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3pvinbkpo.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3iecejsla.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3justwcgw.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3snbrnzrs.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3hdhkejbv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ohaioxwm.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ucecrvyl.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3xjsjzrlq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3nmxrlggj.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3ixanpjej.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3zmwgegxu.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3nnasnwye.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3jsbmvmnq.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ozgbbtfr.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3oudmpjcd.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3vxpxzjlh.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3gasjxsew.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3xwqbpufe.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3byeeagsh.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3fvtbyeaq.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3iptyajxz.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3sdnuiswm.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3lgbizpzj.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3suweknmu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ynuvlkrx.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3wupbykwf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3mpfaaifd.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3jqynnwrp.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3ujzqomki.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3zxemydaq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3uufbtcae.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3yuirhisq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3sgcnsxqo.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3jgvqdrxs.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3evhraznm.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3uzwlwsrl.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3oaxkaigy.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3ijtggwtm.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qqqvwhaq.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3clzetfiv.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3wtieaowp.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3ndgfwnjw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3xgjngsnp.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3hznaljfq.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3jqhhhwyh.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3pxchmccp.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3fhmrqmug.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vcxbndqy.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3dgrwhrbx.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dopnnzms.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3apjjhwca.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3rlghtygr.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3dmlngjom.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3exwgfryi.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3rdhnbwzp.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3aeyihozk.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3crdurqzl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3yymfijjk.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3mwifbfvo.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ljnaiuca.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3xsizcsdg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ucjhowum.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3pwvcacwx.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3fzrnmupl.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3cszlhqrp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3bavzblcz.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3ulwunllq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gjdurmhk.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3akgsaugl.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3nttszdhe.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3pjxrnnzi.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3vyscixeu.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3urytprjf.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3tbkaqirv.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3uulyokyk.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3drzmofsg.html


<!-- 参考信息 -->