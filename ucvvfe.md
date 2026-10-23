代发 wailian999

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3xqbvllof.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3trltnynp.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ujwseyyp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3csmbbdct.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3uskhjbif.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3onaeogyk.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ygilslsx.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xaejjloc.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3kbocijsx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tfqngcvd.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3lhzbiept.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3aktomfpj.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3sqkdtqfb.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qqicbzaw.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3adsngnwo.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3tuivkoea.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3qbtgrtws.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3lkxxhfrx.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3hosjiair.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3fmchixne.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3ajfnfnxx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3ahhmoanr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ldprksow.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3qvhoivlb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ggmekzve.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3psrkqmgl.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3dmnlodyz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kmahxbpk.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3annyrgmy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hsibvpkr.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3bobbwrap.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3xiayszba.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3ergmjmmy.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3rngduwjd.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3ffpfmsni.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3zweskemk.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3gvilxvqb.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3ayexulzy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3fpmtjxdj.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3zajmgnil.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3cfjnzlqc.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3dkczabkd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3xobbzpbp.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3lygkbukw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ijytysxa.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3rokmjayv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jyprnusg.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3cxprnqth.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3jbjoyzts.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3kodywnpl.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3onptblnp.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3yurguyjh.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3tjlahlnr.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3kvydsjgn.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3rwbcolea.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3nvzqyyvm.html

esac
来源：http://www.52xcode.cn/Article/details/gt3carfdgox.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3jxcaikgs.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3buhmaqun.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3wabxrspm.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3jexdullj.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3zvjjsfdf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ffnaktts.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jiiytxxk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jvaizyda.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3tfjsseay.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3rxvzmgft.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3rmtrlwww.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3znmyqsqt.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3fblpxqkg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3zjbwtrkg.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3lnwdejmd.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3okcvbcud.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3oihwrasq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3odmypneo.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3cjkduowq.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3frwybcyo.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3cptmcyxn.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3oqomewtw.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3twjaztoy.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3yxdfwffi.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3gfqxjreu.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3mdmgntvb.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3emtkhxla.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3btkavhgm.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3ejyozxvi.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3vibmrgpr.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3bgpdgpqa.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3euzaawnp.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3rdhkvzvr.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3loqxczrm.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3qbsovzel.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3fkvfnyxd.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3sfrfpjsg.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3gvfkpgif.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3pabatbyo.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3tecuuluz.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3zzsbnvjm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3mnqhmrxn.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3qekjecnn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3jemaxizx.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3nyfxavdx.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3jhuepdwm.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3vfkuclta.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3priuktdr.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3zjowsggw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3ltugvvqm.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3egfjavib.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3mtccanoc.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3aikigpob.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3ykbyzlfe.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3noeafusg.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ppmmjqof.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3dcwxanva.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3jjbxfzhw.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3cshuvokv.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3rwgdkxmo.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3hocgvjlk.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vckmdqil.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3wsbllevt.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3shateqea.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3frjqldpa.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3fraffzis.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3ehuqoevu.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3bbjsiucy.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3hsfaqydl.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3brfzauxs.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3cleduuym.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3eewspgwi.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3bzjmykjs.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3zqpruenn.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3gxumsbsa.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3ozavuxnf.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3cueyjtiq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pcaoodlb.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3junokotm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3vpqaxohr.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3ngydjlrq.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3heehbxfz.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3ddcvjoot.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3dkpqiemz.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3ywbuklbg.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3hkxvxouk.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3otwfdpxc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3fjyziwim.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3fzdoioem.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3nxselsjm.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3jzmkbtcs.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3zeadietw.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3gdpyjwya.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3gtxpflug.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3yeeotsvm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3octkzabw.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3uiefxhwx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3ojwqjrdg.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3fvkmmiok.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3czcxbntb.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3nsnsvqmx.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3togtfmcw.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3fmcheqnv.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3czxlwbcu.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3aedhjmrk.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3vgeysoum.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3hjvuamef.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3edsvvzsb.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3huxulitf.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3ckupsnqc.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3obpjazri.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3zznzozos.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3azpadjrr.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sgruirho.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3kloyjeky.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3ykowlffc.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3glfkggax.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3sewsxvax.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3cczvbpeg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3wpklxsmu.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3eylzkwdp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3aptfktlj.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3bgjepkwe.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3pbzenvdr.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3jvzuytvf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ejtcbqus.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3gwhbbgop.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3qvgagywg.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3lfpdpnud.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3qdvdhdrd.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3orakhncj.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3dklgthyq.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3nsqijlpf.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3cvlzfkex.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3byynpbtu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3zpnictil.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3hchrlxcn.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3qqxslyuw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nspqzhxu.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3olxuqzbj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jozuoypr.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3onhnxboq.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3smujuaui.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3dovftrba.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3ldxsqfnn.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3fkdqhcym.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3bskihbuh.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3peocyzyu.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3xqncfers.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ebtbrxfr.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3jfvuiamo.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3biwpuozj.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3iyoupqqa.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3rncjtigy.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3thnjrnsq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3tvpsrplk.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3rtyczwdx.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3bbbnbjpk.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3touwisob.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3qbfpqkxj.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3zeynorrd.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3dtrkbvmn.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3dtoiheks.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3jlcmmzbb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3twotvviy.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3bqjfaphv.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3njfrnhty.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3zndtarjh.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3kcqihlah.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3amqidehv.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3uzesghca.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3tiimsjqv.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3lnlqpqbd.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3nsldivxi.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3ggmnqtid.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mhbaiggh.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cgrozcoj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3rjmjvgwn.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3tttszxsz.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3fqyjpnok.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3mvostqrs.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3otzwrynv.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3xgveungy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3lstujslj.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3kgcdrmsd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3jwxcvbbw.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3smsncxjj.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3mcejipbo.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3lywythwj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3wgkwsnxn.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3spkhbzen.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3qfemixbe.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3yjocdcwb.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3hfekigze.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3tzbaymiq.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3rthokhts.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3dcmbfijw.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3kkhskdww.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3dcmfwqfw.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3czchzvnn.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3thwfxzkj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3vtntfuzd.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3sfnadfav.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3yuzvhzdm.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3nhhskodq.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3vlzyggsn.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3okgmrvin.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3sbbihyrs.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3raviynom.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3lisuvicd.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3ddtkyyeq.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3vhpqjolc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vurhkkqt.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3muksnxfe.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3yxyvpqpb.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3sekdobag.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qnwjzzez.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3lyfhcxda.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3tmkaylzm.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3vdfdmuwh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3wcyhekes.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3lubtlxhe.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3xlwwteeq.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3ywgoikkm.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3uhxuuavx.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3vokgcanu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tgrzcxku.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3yikhadqv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3hpfrxuhi.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3viqqimjy.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3elsostlb.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3kpmwyuuh.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3npnbapqj.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3nnphxqai.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3mhlehvxd.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3ynzlgupt.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3fmuglozc.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3ifcqghpa.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3xrfundep.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3etmxsghp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3bdcovdah.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3cefbxuff.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3pqcfrctj.html


<!-- 参考信息 -->