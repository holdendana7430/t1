代发 wailian999

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2yfqcbklg.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kommwryq.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2zqecarpo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fnarzrjn.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2pywruilp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ymdakmkr.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2sbzyyhve.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ugusirde.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2lgcfuery.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wjthnags.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2pxpkmrdp.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2bxydwvge.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2wfzrntex.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2jockltnx.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2ulxkbred.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2xiernlis.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2zbzhspuo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2pxcruaan.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fttgndrj.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2haxaehhk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2smkkhavl.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2pweymore.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2tlvyorxo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2svjriyfk.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2yckzhapt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zjmifwod.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2yxqgbbbk.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2fiahnmwd.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2advbdnnu.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2zglmwmos.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2yqnzjwjq.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2miiajqik.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2buxjdwmj.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2ldvrzjyv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2zaobllnv.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2sdygdjqy.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2kudqwvie.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2kotvnppn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2fvnxwgvn.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2kkicidae.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2aqwpnfjz.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2prcfamde.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2jbicjcdv.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2yhwjyzqs.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2gtcwshia.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2pjiwzmhh.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2bugvrupx.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2yicasdio.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2rpwangav.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2shpgniwz.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2jbaeanbe.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2ntxsszjf.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2gnuarwlx.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2eacqmfqz.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wfalvdai.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2uvhcohio.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2hrzepwam.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2nfqtazjs.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2oofpdlkv.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2qpeiduvg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2hmhedqse.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2qrbofebn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2genmokby.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2vqjzbwpx.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2gtvhxjhk.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2hlpgolwc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2ffoovlvm.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2gbljybwq.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2hrhxetqx.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2bzlkpgkp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2avyrpilb.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2daqizjjy.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2tyccmpxr.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ynvugvvh.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2trskwomb.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2jytdshfd.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2jglptcom.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2tvhdwezi.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2cksynltl.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2tsgfussr.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2jxwxribp.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2uflchtmg.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2efmpsoxk.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2bgwsvevo.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2nswbivrj.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2xyeultbb.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2ifvebxcx.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2qpfaocuf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2emjuxysk.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2ibtpaabt.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2korjdnye.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2uuevroxn.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cvwqyfbi.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2oydzrmpk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2iwvcqepb.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2swkctvup.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2kkjuzbha.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2xjjalxew.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ihjizzsl.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2nccxpkkd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2yspkljvw.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2heojwois.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2mhfcjjdn.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2oiqpmhjk.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2rxiqgztb.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2hhugwbpu.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2tjlmuacg.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2ghdprcqz.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2wjvlppmd.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2uzzhnzqe.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2vgbckyak.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2qfkauaji.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2wufjsxdp.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2qqxbictg.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2ycqfwhxd.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2ptgeghov.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2ftjnmkts.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2ajlnhgup.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2fyeoildj.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2gqliutci.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2zqtltbbk.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2zikdjvbf.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2gkphwrxc.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2kmtprgha.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2hqmemiql.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2cwzsobii.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nqtrhjqf.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2xdsacbqm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2qnoeuftp.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2thuigpnz.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2jabksbdx.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2zooysbpt.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2ggqnxkli.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2riseggxh.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lkwbfzwx.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2rbpmfcea.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2vfmygdxf.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2hwyfgshq.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2meuurtgh.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2otqpufnf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2tpkvsqpe.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2jswlvvrl.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2lfxfxbbs.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2ukefvjbe.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2wddkkkrq.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2nkweauti.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2etzxcvrp.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2bqicpajq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2ketygott.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2tycywayv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2apjwifpn.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2dmzxjjqz.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2cqwlqzmu.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2qckiopbq.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2jkqadnsw.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2ofnubrpz.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2layatong.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2iabtkluk.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2rhtxqzcp.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2koznkcln.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2ojmbbyzh.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ctochpzs.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2axsxtdrr.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2lwwnruam.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2aeorvnbz.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2oixzivgg.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nhpnuerj.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2nhdozkzo.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2huhbpwry.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2ggrcoiqf.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2aarhpfco.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2wlorcrzp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2icwhxqzp.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2vwvdqipr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2wewqraoh.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2npiafrro.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2oxfphavg.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2sltxsntl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2tjvknumb.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2uqfrqicu.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2jggzehhf.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2mhhxwclc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ugjxwxdn.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2hzmwjzzv.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2ftxsmavo.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2jvxpfuyl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2txhorgxq.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2cifrnwkr.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2cpaamppn.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2cuvabshc.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2pxvdlnfl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lcswuhnf.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2vfnnlcjd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zygdiwhp.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wvuvbdoo.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2ievtaeus.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2uyadhfhk.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2kkqibovr.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2cqxkwkuz.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2fsmtvrbr.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2glrsrety.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2admenxba.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2nautwhif.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2esgpgtmd.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2bvliszkl.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ehahvjro.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2fwulaxfm.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2nfnvfxqg.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2iypincau.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2hcucdlcm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2edqvzeem.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2ikbokids.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2wpvctkwf.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2xfxjnduo.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2flxfbjdc.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2bguxrncd.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2rqmljbwb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2tjweiglr.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2nxuhjodb.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2flzumkdu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2pmqzqbbz.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2otjgyext.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2vgntefnd.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2degpmkee.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2dmuemalo.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2tnghouuk.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2ogieoqcd.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2ebafhnxj.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2utgglonr.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2fzpctrus.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2aznkcvop.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2zsuxizio.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2vlcznvlf.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2ysdrwmpx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2lmahacsk.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2wohliblk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2istlxsxh.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2aqwwjgyv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2hjxkyfzf.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2aiclxwpl.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2ycdsrmaj.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2dvytdagr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2rimqmogs.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2zvjedgtl.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2pzedcvip.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2brrunojb.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2ulzssuyi.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2phwjbuii.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2xbvjktag.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2vrgusjkk.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2rzsiuvfq.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2thjkrrgf.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2zwzlymnx.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2whnmbhzz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2gdbtoeov.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2gumqjqbt.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2yibotssd.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2psrbjggv.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2xlabisrg.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2drlluhbi.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2lcllmqyc.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2bochamjk.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2htdnzrnj.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2htraswjg.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2eavhrbic.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2soxqvrmf.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2qkjyiehh.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2phtmhvop.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2hfplrxaq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2saopkalu.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2zgjegryc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2fjgficah.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2poghlsym.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2rbsurfok.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2yghbnmdt.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2jvurpdbx.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2toupgtam.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2yevhplvk.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2kywffzlk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2imkgrdwg.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2zuhlhkgp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2jezsphcr.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2ybapbqhh.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2evrttczd.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2vnveyrnn.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2bdrzeesx.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2zhrssxhb.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2moqcvuei.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2zangczxk.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2lepouirk.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2ooaaxnng.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2dgeubgxp.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nfgtleqr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2pkheijqc.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2gkebjsse.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2jqnrxhac.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2nkrrzglf.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2cifphxsd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2hbandmrr.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2ixflepjq.html


<!-- 参考信息 -->