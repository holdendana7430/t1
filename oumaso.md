代发 wailian999

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3cmejnplx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3waurlwsb.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3lylxfwwl.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kmgqqdua.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3hfrrqyuy.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wnsojlvq.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3wsdjqulq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zdpeqwll.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3mejacqju.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3igrkptxy.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3nbggrhkj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3xafdmkbb.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3cxlwkwfn.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3njlseysl.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3tzgxgstn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3qvsrjsvl.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3tymxvxmn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3dfvcbljr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mgdecmpw.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3rupqbnko.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ypkfrdmz.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3leqqjflk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3gkrnfzza.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dssordsl.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3pljrhbvx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wckuohve.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3teggjdgj.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3ptxnpfqs.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3jzffobwe.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3bdqttqxw.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3qefnxvnk.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3tgfhiisp.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3puzhelzx.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3vgpmcvrl.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3qitbmjdi.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ewfcibvl.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3gmjcgxgo.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3vxabckuz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3bjelfsfg.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3oeowvkhx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3pydcxkbf.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3ieliabhg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3yrasejku.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3tqawkvqf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3jomvaiyn.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3bkkcdsxd.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3mqzmkawg.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3vddaeryo.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3psjyfwtf.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3fstnglcf.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3bbctyibd.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3lizumhqb.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3bugujnea.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3kyrztcfy.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3nhqtwepq.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3tfvftmls.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3usyyikoo.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3inphfany.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ihkbyiie.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jmrophap.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3ztqtdkrp.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3bczzudow.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3vzkbkiqx.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3qdlomsic.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3lbnmdvsd.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3hcredlfw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3sowdalzz.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3mtndibrt.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3abqnrfpl.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3kzaoevdy.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3bnjxkfcq.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3pbioyhxi.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3bdekmhuw.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3kruqhtli.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3fslpcvsq.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3offninwv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3wsqpyflb.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3symeexjo.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3itkxrgwz.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3apwfzejg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3fmixfojc.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3xtmfqicd.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3cfcriepp.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3wjdjfojs.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3hheuwzxl.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3sduehnco.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3hrkbbnal.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3dysnuosa.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3vznaxzlc.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3cwjcynrl.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3gdocusth.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3txqhxeem.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jyfxgijq.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3ehigpxfy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3gmokdhme.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3vzzlzhux.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3gmaoosqi.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3aoisprft.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3hpuoqxur.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3mpqtkwbx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3edmqwyst.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3jastwxkd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3jukacnrd.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3cvvecrhp.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3fsvqqwtm.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3orjdoiot.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3ggqxuwqk.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3gaacsmpm.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3utupbkcq.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3pwwjjeuk.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3qpbmdmmp.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3jrvlrzmu.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3hnnljhkk.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3vihqlrie.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3kneofcpu.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3dlqmpjjr.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3ywotzlsg.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3jdhddvwx.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3wcssucoa.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3zbysffom.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3sqlpngqr.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3ltuifihm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3lyecfrjj.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3phwvmxqe.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bypasgft.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3kfuzusfq.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rxajkicj.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3aepxvlpp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3xihitmfh.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3ccwohfyq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cdqkwskg.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3iujnezhz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3nsizaqqp.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3bymkfwyr.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ugncaweb.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3vflcpqmg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3hpdcsfsr.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3jjpqboya.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xkaifwcj.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3jyctihst.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3vmfvoncg.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3oewrvors.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3tyrzndhd.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3pwyixjjq.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3whpjdugg.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3bzrclhmr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3wklazhla.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3xxtnaqaz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3gfmcfmag.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3pjsejelj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3qccjbpry.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3ofcjibcq.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3bmjwtvhb.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3wadxyyap.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3drnbslto.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3yoiisjjf.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3bcamhrch.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3jqfxhaqx.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3yhjkidgr.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3iaazeqdz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3oesvpodo.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3raqrrnlo.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3qtwcimup.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3ktsqjqym.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3cmbuspzq.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3snnqshdh.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3neurfckk.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3sxyiwfqa.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3obpfbpba.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3boywlnki.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3fyyfjjvo.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3yyfsxfcb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3jrfskewl.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3zcveycfp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3lzzxxuxc.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3isgpbocd.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3jzpdmpvp.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3cacefsbl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3opnxjvbi.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3sdyecsse.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3cyaierfm.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3kewvwati.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3iibftceu.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3aeennvhx.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3glxrblgq.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3slsyjmcr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3gtqaawuy.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3zkwqefqe.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3ehcjuxiz.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3pukduaif.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3pxkaflhx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lajyqfhu.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3mtlftmtu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qixvhogb.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hcmfjksd.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3osqzobfx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3wfvwenlv.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3uhnjxaop.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3kcehjhqt.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3zhsxtzti.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3tjgsoucr.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3zubkzxhp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ncylxsdh.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3pgzvplrw.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3tbaixwmz.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3irueirxs.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3mdrfphot.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3ppjzwzrx.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3iuvanqzo.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3biekjdwu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3ahzglwmx.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3vaxffqbk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3xqmruinf.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3vdnjmwun.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3ftafjefn.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xdikljon.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3rtafpzyq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3fehhqdec.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3nnmuskpu.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3hawqbavv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3vphhuyon.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3njwevpju.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3jdkxvsee.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3xszkvkvm.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3lchzpaiq.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3hjikiwrl.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3fcoulpdw.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3fofnlwtb.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3gaffqrag.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3tjomcgrl.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3nrohggmp.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3uxfnwhjj.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3oazdijqp.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3fcgdjkxx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3jnvhuarj.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3frnczyck.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3epuaitel.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3onzadwml.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3xwuqylpd.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3dbkuqsvi.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3jpmpcxno.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3pcswdrkt.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3zafqbsxr.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3krmpbmpc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3grexfolb.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3vshadqvh.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3xbzdific.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3ncqzjiss.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3cfddadjg.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3gcdxhvou.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ohgkvdfh.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3ibeyhkyr.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3klnzfabb.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3qqgzontu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3thbwfdnc.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3jmwfdhnz.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3hydwdhlr.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3hkbukaaj.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3wxtacili.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vwmuuvzp.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3deucfgis.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jdzsgaae.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3csinhtrh.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3xtdohanb.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3uqdhospw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3fsnhaovx.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3qnhxhsxs.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3innpogke.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3tbzipxrb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rbabdxfe.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3bwxwtafk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lciryeah.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3qqjbdjbc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3iytxeclj.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3ritmzuqz.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ekzvtlph.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3riujuxdt.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3jvgshpbc.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3arfenjov.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3inqisktw.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3lkgskjii.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3gmcpdmyy.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3rlkjdejc.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3yfjctjgm.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3kccmjwfu.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3lkkzidvt.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3wgvwqsgg.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3lkmrvhcg.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3pahvawls.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3rhqfiipg.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3norixoax.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3bakqrgko.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3onufofin.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3knpyfgfi.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3npgytmgj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3grxrygah.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3jpgfmxmg.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3zoerzctm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3tmhksymk.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3wlgywxeg.html


<!-- 参考信息 -->