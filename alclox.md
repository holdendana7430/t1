代发 wailian999

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2funpyxoc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2quifyrqo.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2bhnztzar.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2zzxybivx.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2gvtxqiom.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ihzdomyg.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2zoscnrwn.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xttdjdzk.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2pnyawnzr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qmozpdnt.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2lvbpujyt.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vyovxpgr.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2otybcesr.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dvdouykn.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2bfkbnpol.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2lqyovfia.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2xyguzjck.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2gmitxgqu.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2mbhecvrl.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2raonvfrb.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2rvbdcntl.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2xjiouqth.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2frgkwnju.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2honuljua.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2iwdamcka.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2uledfuuf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2ckqcqhsy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2txinilxz.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2qhzrfjov.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gfuansfl.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2hpqevmvr.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2lqtrnjeg.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2hnpqhvjo.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2gxkwyvhu.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2jhljowyk.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2tepvfsdm.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2msjxniga.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2hdgfvtxk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2ntecmrbj.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2ylhnmcmo.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2slwqyulz.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2ieujnegu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2rmmuddqz.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2gvkuchok.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2tdtgdrnp.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2owreciej.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2bahlkchu.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2hjroianx.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2dqicwaos.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2fgrlhzcw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2qmsikfhd.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2qxmaaolj.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2yywmdvby.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2sjxqduea.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2fmwsobhp.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2kgvsrwqy.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2dfzgikdj.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2mgrmpeen.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2zsssobme.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ymsygznl.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2zvrpbicx.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2bjzuycmc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2snwqznkg.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2hqcuzbkk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uiimfxzt.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2psrtlqow.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2coshfevj.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2upupdpjh.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2gcvwwwfm.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2pklwycyo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2ialwowbq.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2qwctufmn.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2bpkalyfa.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2lklrvpxy.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2xpanbyzm.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2echzotpk.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2vlquphzr.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2qkoancdv.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2rchqkoxu.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2qvmisgcf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2kpkwczwg.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ogbwyyxy.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ffwzktdd.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2yjjlzjyz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2zownksrv.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2cujrahvk.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2zhrxyhlx.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2qkpgawkh.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2bdpwyniq.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2imrecaob.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2wfxnlovr.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2suuiylul.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2xtgpdhzk.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2pggbecvv.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2jaomvzgq.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2ixbwanyy.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2yldgiqhe.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2zsskctxj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2exhwsldj.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2aeqhkpxs.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2qitevlhu.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2xxbaihfw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2pkykgnyl.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2mfakpgcp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2jooeuolw.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2ovfudtib.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2mbflxngx.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2adlarcpm.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2lfsbyqnl.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2ehfwhjfn.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2ioplxtxl.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2xwrpptzr.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2somnwonb.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2iavaqrjj.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2jqrhzxgc.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2avnpjkhi.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2fbwetywm.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2uccaeahs.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2gefhhoju.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2rtxomyye.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2pysgkons.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2fuhvyebb.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2jnyerbqm.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2biqatmcz.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2mnymxtld.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2eetxuigp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2gfeeappv.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2mukhcvpy.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fkeuzlxn.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2rgeazmia.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2aylmpgiw.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2tmixvszp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2ygyzsuwq.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2mwiucbgj.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2zdmqnrxu.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2wvfcfkyn.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2haxgbwze.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2uohdduhe.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2izcrlshw.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2hymhffzb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2xmxakvar.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2zppkyfxp.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2itcpmclw.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2ndlxmlfe.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2cyrilmkn.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2xqogxdyu.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2asjrnzln.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2exwziuzc.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2wylafshy.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2mroitbvm.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2okrogkab.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2soasgdwh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2xuheuttt.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2tghbkfie.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2cwuqlkqy.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2whzquggg.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2iyefzylj.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2tcufldfk.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2tlnfgdad.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2umcluinb.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2nnbszypi.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2tzyotfoq.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2npinouol.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2ihbxmwig.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2jdjdebuq.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2fvduvbpl.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2qwnoejdc.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2mupeuzig.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2mkywgxli.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2kyxezetm.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rqagydls.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2gpehcvyi.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2rdqaagwe.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2avdcodvg.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2kxqkdakw.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zfnymsmo.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2ysnhhwqy.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2tdjqhili.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2syzngclp.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2fnhhtozi.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2ztijdikc.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2bzaqwmxo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2kpplwlts.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2riimbphr.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2genqganh.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2icoqkvei.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2mcfpmvmu.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2hoznvncj.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2wycvpihz.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2xshwtwhz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2ykkwbmha.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2jepyywkr.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2iplvpvyn.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2spwqyeep.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2cmzsmlfi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qkbsxemo.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2bqdauiyf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2inwrhmrf.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jmkmgptz.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2dzbrnbqm.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2pzkmxqol.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2odcxhzxy.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2hdkbbaxc.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2dlarmpsr.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2jplbgkcf.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2peqlvoif.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2lhrdvgxp.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2xhkhklyn.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fdaqpewz.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2yjufjknl.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2qldnhzxb.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2istlosyi.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2gdqobotr.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2nyntevrt.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2oafgulqh.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2rmryfsxx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2dsumjccf.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2bbccbsbi.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2bgzbteyl.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ugvfvxou.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2zmrysgba.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2xqoxqkhz.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2gykbqfbl.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2pwofbrjd.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2wwmaznwj.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2yvhnjpvo.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2mtgqbfzb.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2zmjcfpws.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2dyroadbd.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2zdxihuir.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2lcllszal.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2mrxkrctf.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wcrzlsge.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jwhmkuvi.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2ppxadiqu.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2kfynbefu.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2lmldwygd.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2lqznyvkw.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2kvooxnka.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2snltixbc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2kijmoabm.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2fimsebsk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2ciylhxla.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2widtnlyc.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2ngbsgrps.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2hyqfqcja.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2wodqeabn.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2wnutxsez.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2smkxlijg.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2ihcqkkiq.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2yimmduey.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2yizhjjsc.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2lbdiswcw.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2ylbghfbm.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2egazdplz.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2hzaxasub.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2nyrxotou.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2jesdiwzj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2eeoyoznk.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2pgbbgdzr.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2nfusnptp.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2nxbukjud.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2fyuokxpb.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2abenykqy.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2wkiobeqv.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hhncbocd.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2salakukt.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2erimrdos.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2exusfqqf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2lhvquuwj.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2rxbrfupr.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2lfaumklq.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2rxhqjfel.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wfbcpeeq.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2eoacxpwx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dqpbfqjz.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2tcxzlfkd.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2xrkickpf.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2ilrpwyeu.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2zetqysip.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2szxviyhr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2qdklvtcs.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2yaaztfho.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2smljacxt.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2vdyknjgd.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2fvpgfkzk.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2foxpabyz.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2wwfvzpiy.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2iwhrklpp.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2tlbzmusd.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2fqgpdmuo.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2jogusqay.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2rzpuaqci.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2hggzjkjc.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2jbhnwkzn.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2qmfduviw.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2bejnmzud.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2pcrlrjqw.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2gfkdwzsa.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2tzuvuswg.html


<!-- 参考信息 -->