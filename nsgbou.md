代发 wailian999

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3vgdnfcmc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3qznbciil.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3yfuxiaya.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3jlpzfgfv.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3igjmxgbq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wmrjbtmc.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3migolcrz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dvsbhasb.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3nadvxqfu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xtebtzja.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ilnkvjgt.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ymodnlfv.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3tkljrapf.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mpthbtkx.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3zuabgolu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3paxjdruq.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3tycrwpot.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3yngcqkin.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3dihclozn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3vpscwxlz.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3ytfrjnhh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3syncftwg.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tajvpsvk.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3lvpmofam.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3esnqtjha.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3xjueucgq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3ewckzmdb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lijeplzw.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3xcdvtpbh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xlegmmii.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3dnvkvexg.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3expijrpx.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3fwqescru.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3rgqbmnpa.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3btxfwbsl.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3pvqppxst.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3qdrqtnqr.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3dwlanjyd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3rfbsruyv.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3iwdjwjuk.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3ykdcfqjy.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3ynnijacb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3zrqzpinz.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3fgrpisvt.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3gxkgoouh.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3dioivdzd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3qjrcdkpz.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3sqmrfjuk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3iubexflr.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3zlhvgiob.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3uwcguroh.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3dioimrqy.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3feuzhewx.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3puxzkzwo.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3vtdiwjdm.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3uxzhjdwl.html

esac
来源：http://www.52xcode.cn/Article/details/gt3olsagrvm.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3fbbvggxy.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3aoozuhdh.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3mqrazqbs.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3rnzhxjcl.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3cfurgxhv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3htdftrxx.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3sssakoxk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sfocelko.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3mzkqqkte.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3feojjhcb.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3gdouvtqv.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3qacufolw.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3ibfncmzh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3qhilluyh.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3lmcxhyhd.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3dahcobgk.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3usluelzt.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3zghzorlp.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3qlrgoqxo.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3rxwxirpl.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3offnenep.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3nqztxoys.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3kqykdjkr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3aowkpujs.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3fixgblau.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3jjqlmngc.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3qdyndozm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3nejwodmi.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3rjdvxwss.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3ozormupa.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3taxrsegz.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3pkxqxjti.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3gxhxugop.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3osgqgjkq.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3bafudaev.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3ypxczdnb.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3evxckjrr.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3dmoschtz.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3imgzipbw.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3hovgexfq.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3rrbjngra.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3pxctjvoh.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3ytzrauyg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3phszzbul.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3qmpclybp.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3ewlehurb.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3mbzimldc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3kaaautbw.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3fvbjtiqs.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3sqgtmtkr.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3usykdpop.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3pnimafdu.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3osiczggk.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3gyfjeveg.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3naapwtpz.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3yozjfyiv.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3hnmufmhn.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3cazfznnf.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3fqldfvak.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3uxnozhrk.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3khztewfi.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3tqxadklh.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3daaksxjm.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3dohblbti.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3drzoqkzf.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3exqyotxb.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3kjtcmxpy.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3trdjfpiu.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3rkefqsre.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3ddtajyvd.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3upkqyukc.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jzvldatt.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3szfkhepg.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uykciwdp.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3whyokymp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3yprqhwqc.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3dzpmohvi.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3jveogxfx.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3qpbbyhij.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3cjxfgdrz.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3uibbonto.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3shmwdadq.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3fdvtzpgn.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3xqteokgr.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3evxfwjti.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mmblarhj.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3ebrtixfp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3dajtvzdt.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3ubngsism.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3jzhodpgq.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3gehmpbxs.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3swxvvptp.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3neiwvksi.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3onqovcwd.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3fempaslc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3glyssmll.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3dgetonjp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3ayuapyyt.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3qtqdjeuh.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3kabkorud.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3psathbac.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3tznxkpfg.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3tmwknflv.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3fupwjhma.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3bjzvzybs.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3xmfiegii.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3lwbjgyll.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3uiqxrlvz.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3wqpqquie.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3snltohfw.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3rsbcmdlp.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3tcsymkzh.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3mzlmgdlf.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ewtxqbzt.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3koglsoxn.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3sjtgsvli.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3aqjrutsn.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3srgjmvft.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3apgltzhv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3fuuramws.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3ekwddkau.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3onbpkyob.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3qskldfra.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3fqoofbub.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3ooxzpwjt.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3aewzmozr.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3uejckssa.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3fjzzccqw.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3yfwaxxlk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3tsdkcfwg.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3bipwikwx.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3equafhzi.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3ilomlnse.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3jkwsyivh.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3obfaxrsn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3lmupiosi.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3ywknoxio.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3fapzhjze.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fyfvdyqy.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3yarkyboq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wtbteqnc.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pmzfuaqn.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3puyiegmz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3tnvdbtku.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3xgepebpb.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3hcrausfq.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3ptjjyjnr.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3wvefszxi.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3dkljizyt.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3gjvsnsyc.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3dkecrhdg.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3uwmyuwzp.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3suiybxvk.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3actstpmx.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3btffmqcj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3barhnqho.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3abhqjlae.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3widnkvuh.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3plilgcsx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3gyoohcie.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3lsmynmxr.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3ygpfwjuk.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3addvwjpm.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3kbwjiapv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3lzombkif.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3uqfkomzl.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3giwhjvvf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3xtdkwkyt.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3rmbbfbvq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3veiqqctt.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3tcfnhevd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3ldmgshnq.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3yvrjxfvo.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3ocawxtbx.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3xmqfnezk.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3prkqqdwv.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3nfeasscd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3wvxenokq.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3xmwgksce.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3vktaesfi.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3txbdxslu.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3bylphnoe.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3rsgizfio.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3hzodaohb.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3xlivzzui.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3dwzitrlu.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3ozpkzjam.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3nkpcxcca.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3fktdqyoy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3fopywtrr.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3rqvlqsdu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3lojlqatb.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3ukxvkglg.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3afdmecgf.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3dilthocs.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3mrmsztfp.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3wiwbekcf.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3whtymqav.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3qhcqlpqn.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3uwbdvgmq.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3agmjjqyj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3dowilahh.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3hqfoitib.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3yuopsloq.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3lyvruirv.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3bkcygbuv.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rkmsqrsg.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3bywbcwkc.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3ijfrddhw.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gfsnpskl.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3sueyndcd.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3wzdzcadu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3anonecfr.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3udpxpzte.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3uzpllwsy.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3sfdipfkq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hyfnpzid.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3sxjfeild.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3aevjkahk.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3xiijczjm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xtfgmnmc.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3judhmgsw.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3akvbvplt.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3zirkzahx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3raaflfxf.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3wmvnstyk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3phfagzjo.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3zerfjxmy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3zrenilxk.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3xbjgmxls.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3jjaqbzty.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3wtfrqsvv.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3pqfrlham.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3wjsmfylu.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3mlapgvwx.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3xygfzyyc.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3cekrobof.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3hhzxsaji.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3qajkqzzs.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ohogeykk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3taglonhw.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jdliwrtu.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3xjodvtbo.html


<!-- 参考信息 -->