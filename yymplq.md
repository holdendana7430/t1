代发 wailian999

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2obnprzbq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2trysohss.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2evnytkos.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wbinxtys.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2phtcujtc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2biluuhgn.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2dkbbipmn.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ewsvphef.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2mgjbyevq.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2typvgdzu.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2zqzzuwjb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2ncqysopc.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2uakzcnpi.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2efroltwd.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2yavvuglt.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2kvnfgbuj.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2qbdllqxk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2ldowdued.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2thqczhxp.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2bmcxylym.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2fdvhbjxh.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2fmhoaqso.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2xcnjqjui.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2appxjors.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2xpgnlgvn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wwhkiknp.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2rwmyjffh.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2xbwhhazx.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2suxhzcty.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2vdyqenrl.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2jkenlcug.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2ewvqwszc.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2rpunizhh.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2xyoavvbl.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2isfyrteo.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2dnwkswxz.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2ywfyjdcn.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2wwsasldf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2bmckvdki.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2gnogpkje.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2eyqzmvka.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2xktgjpko.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2jdmekwye.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2udcxywpj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2vumrdwxa.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2shwmtnno.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2cnjwwnsk.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2tqxuikbn.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2arstztjz.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2rifetgne.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2tfmvhgmi.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2jpmlixrj.html

esac
来源：http://www.52xcode.cn/Article/details/gt2cppjdotc.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2ouaqderc.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2xhstzoww.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2rncgczdm.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2dkxtnqgn.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2tncklwch.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hbkwurxc.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2rdkztmtk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fqzkzhmm.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2kbiiffny.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2gzamfjwr.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2llrtrtxm.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2akvfetqo.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2rhazzdjr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2nilfgtip.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2oylnpnty.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2mgiuofod.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2ccuaurkg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2axahpbyu.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ubrwzowv.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2arsktsdc.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ajmfpkjo.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2zlcyvbex.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2kfqpmjua.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2ntrelfre.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2dwnjkikw.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2rgxvxwjd.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2qarlsjop.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2hvahktqx.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2xloaritk.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2byeryapo.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2gngtlvbr.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2uzyzxjwq.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2nwzdtmll.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2nqtdulmc.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2iuhlmqrl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2yamtbbev.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2dydctkex.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2iafszqeu.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2buhbtlpz.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mzfxiqyi.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2rjxvkoah.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2kgukzfec.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2dywhztij.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2gtqukvdl.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2jywrkjzw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2hvsjagba.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2eetbmlyu.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2rlulzaes.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2yhoksqex.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2ymbqeszi.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2sjwjubwe.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2ibjbqrhp.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2jwfmcvco.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2yqeneyjm.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2wviqgpep.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2kmnxhglx.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2pgsnaqag.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2phvnocki.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2kwyyxrkb.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2iszzttoe.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2vunxtdyv.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pdqeftbc.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2rkvxkfio.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2uahwqpul.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2dqmxmbmn.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2ysxxhyhn.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2gmproggy.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2kavfcdoy.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2hgaoydqe.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2emvexigf.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2dcaimcac.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2xvckoaqz.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2noagimwb.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xyyqhnmu.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2zjxjgvhq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2pnnpjtqn.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2zulhoglb.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fqxzukpj.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2mskwszyi.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2sfpbnzsr.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2alzsloos.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2gkablhiu.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2ixtslmyp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2pzfpmpak.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2blvayjzk.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2klfswkfq.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2wwgxqrqx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2qbjxhgdz.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2pvatuldl.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2kmzmmifd.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2igsvacqa.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2tvdkrilb.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2tvredxoq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2ombsntsk.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xjxtqrqj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2jozpsagr.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2gvwexfsv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2oubuntyq.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2uwvdxvnn.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2pueofvkv.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2vohopesy.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2hoozrnum.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2swesvuab.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2jrcdsksx.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2bxfjubgo.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2zfhcperj.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2lhihabxv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2xhuqvwrk.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2ozxkdqij.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2insemizz.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2wrczkmgf.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2cgvjrweu.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2tefntcod.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2elhooycf.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2jskycwsg.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2ukxrxvjn.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2bquheudx.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2nxjllxdl.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2uwaguets.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2nmxejtsm.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2cmqbilcm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2gawgdeyi.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2cpqvwraj.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2lihtabqf.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2qyaebfxh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2orejctlo.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2rinhilfn.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2tkiwmfcn.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2fioxfbkx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2cywjxzif.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2xzrxethx.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2xqroilim.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2izjwsvml.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2hdmfupqw.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2uzbtzblk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2mshmqiju.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2tzqzlxtm.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2lrnxkoub.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2heifoaya.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2uavwjanp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yjuddwda.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zatlxcgn.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2hesxtmwy.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2oprozhzl.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2fudnkuwj.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2pecjojns.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2agxtbjtv.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2mbfwupnc.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2jglnevti.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2tatzmlok.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2jlmopwkf.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2styuucxz.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2yktgjnbu.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2guwvdzro.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2tyimrkrx.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2oxlckiyw.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2vykieikl.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2ibxzxsln.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2ufvmrcsn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2hgatozpo.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2cmtuzyej.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2zmanqjes.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ufjjaawy.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2oxkrwaki.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2bjkrmupf.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ohrfcelm.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2hnpgrqbq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2aocgrgir.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2xuhhivxf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2icmdsjjm.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2yczgyudd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2grjaacim.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2vyitfxiq.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2baflodiq.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2wzilpmsj.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2ddhpfdit.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2krgumumh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2hneaxxvv.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ghiwobua.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2ightojvv.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2vimbpsbo.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2uetorwve.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2oxzbfrac.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ryxjjkrh.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2etfbdmxp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2yhdtnvvo.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2rfksmjqb.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2jkgudqbo.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2hjphakph.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2nhulwbxu.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2hfcwaoua.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2neacdyoq.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2eqwiockh.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2grmjsaxd.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2wnssiraw.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2dufevcni.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2zzlbjhbs.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lknddhcy.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2jsnlkoqw.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2wbaxwejn.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2ydwmjcdz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2tumfpopy.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2gpcxkjyi.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2qbtylthm.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2onhhivtk.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2tkgjhtkm.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2neixhfww.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2jrcwrirx.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2hjmbvfin.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2ldmgzimj.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2ytphsecn.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2okyesgid.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2nwvsaqwd.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2eakyljyt.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2esaqbmkq.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2okdftdsc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2eovegbvd.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2osabxbnn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2zrvtovov.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2ffjzpqgq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2vlpvlruy.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2unlesher.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ntzdtjuc.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2aeiwcozq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2hxiwbgbc.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2ymbqncmr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ccvttqzz.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2rpcsical.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2nbctuhyh.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2yroaradp.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2zclzvmgj.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2dghvlror.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2aqqqexzl.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2jqeanrey.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2njdvxsmf.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2bnhkuvbl.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2pswqevbh.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2vosakcih.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2zijaohsz.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2hbjgjwop.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2kfuyieiw.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2docccwnu.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2lcnsmkpa.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2sqoatjde.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2xqmqiirp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2ehbynoco.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2knhdxjxp.html


<!-- 参考信息 -->