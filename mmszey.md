代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2bvilbiau.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2sbcvwjvw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2hpiyxdxh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2osyjfvnl.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2jclwwjhr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2osgnkuun.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2uwvkqamo.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2wnuyozby.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2povrhkrk.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2dzuhaouo.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2zpkmweny.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2vnyqebau.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2xasnopfy.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2gasvmdth.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2whxyaluy.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2zwqufkbz.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2robgfzwp.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2dmeprfrr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2dovjstww.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2qtagrqhz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2shvcgbvs.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2dzukhjqv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2uelwbjwp.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2xgknpmcw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2kcrxsbpf.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2bmqbwmso.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ibvxhflq.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2lnromcmo.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2rurofnkf.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2yqqdlcyh.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2kbwhcgmi.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2zteamicv.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2mmgbqhpd.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2lfwivyxb.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2nyvspzia.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2pqcfnraw.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2quuzhtyg.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2fpqgnsky.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2thqcmwxr.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2eygraizh.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bbbzhwuq.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2vbimnlpz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ymmwfdjy.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2ntuyygmv.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2jmqqrlfo.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2fsdcvoqn.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2zpcfdsei.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2xrgyrwie.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2nclvdmlh.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2fkrhtmwf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2dlzlcldt.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2xdtkvyzm.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2ovvwtpru.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2uquetfgu.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2mphyielj.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ioxtbabz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2ctolfvao.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2fpkjlnkg.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2ydjyecns.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2cqhonxli.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2zkfzpqni.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2bekhrofh.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2xygmowfs.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2tistonwe.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2prpjniix.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2bwbrcarh.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2aapbqtrt.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2qasjvszf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2libsjyno.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2srdxfubn.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2ckglxhfc.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ejqratda.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qbdglqxz.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2azwdutkj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2tscvegbp.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2njhpxlth.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2jqrhyujt.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2ktkuxxcz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2owvtdruq.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2tqghkjik.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2gezawzsv.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2qhddivgj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2ylwylukd.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2nwcyiaxl.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2fkqqjnkg.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2ycfjyqky.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2gqpstbab.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2raknbauv.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2opgrqouq.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2jfqmfiuj.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2symggqmq.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2sondsqtl.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ijauofkf.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2qjfrhrmt.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xijbvwnu.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2cquhexvb.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2oapwojbu.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2jvuxbpbf.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2kjsswrqc.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2zxlmkqjd.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2kxmpcwzp.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2owgllqsh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2oqpknews.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2rcymqajw.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2bxhazdro.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2tzfvmtdd.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ukxdepyz.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2caliniqu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2wilfyxqj.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2hrlfccob.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ubbovdcp.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2awazhagz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2kzrfcmop.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2niwfkfqk.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2uureeliy.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2lbzdfbfl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2bbesdwqn.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2wjolbbzp.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nqcexdqd.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2gqwrhzkl.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2dorvllau.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2gjzpmuiq.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2zqpxhpym.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2cvstfvvh.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2ymbjmnqp.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2twbpsski.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2nhnjjqts.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2exfkjemt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2yfmokbso.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2cfjqxcsn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2upfdjlfv.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2mycwwdyi.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2fmxbnfem.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2entgsqii.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2acolvwqz.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2hmsdukmb.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2ywmnfdzs.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2fkfbkqaa.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2lrzoglbn.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2yswydxca.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2hicofzrc.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2tqgnbtzc.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2nsnpbsmf.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2ybasthcd.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2gfhtkzbb.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2bpupflst.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2pfrykkho.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2ptrdvmgr.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2gwgcdphq.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2txizmpoy.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2vjsunzdn.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2tfqonqsj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2vrzqssvr.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2oaatqwob.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2hbakuofm.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2tmmpeghg.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2zuztccbs.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2alttlkja.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2kkxgxlxi.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2hclhtkyp.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2ocitooab.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2iormuftq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2lehutpdx.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2muvfhdhr.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2anhiavhh.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2sewfshay.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2dixeiwwd.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2tgvfkdao.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2rwzxlkfg.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2eaaggsua.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2cxuailig.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nuyrujwd.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2xhxceaxn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iiljuycr.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gbvpkfoc.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2jxqblvcx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2fbkymyjd.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2fiwlnshq.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2eurvnzvs.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2bnpanukt.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2ighaxjrs.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2hususwey.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2sahclhkg.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ypwhpbne.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2svaggwbw.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ixcwvcjt.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2phlljqkt.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2hqbbinbz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2xmranavs.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2owlakfub.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2aahbeopb.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2romlobew.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2myevxlzs.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2rjgtpbpo.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2huyrkmkh.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2zxsevkjs.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2ulequyfw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2rxjcylxw.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2wwhycafy.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2kaexvtaz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2neqiyptq.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2vjnztlyd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2ifomhfxr.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2jzbmkkee.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2pvvwbvcr.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2lfjsycxh.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2duuqyloy.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2bgsucspw.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fkxnipfm.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2odyjhbvd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2kaekzfyq.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2jovlnvwh.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2pefmsdqb.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2kiprlmcs.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2koeklbrc.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2zpykzilu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2xtapzhnk.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2tsntbtfi.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2xumbntur.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ydguppae.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2psedfmzo.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2tgcnruti.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2gafykahx.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2zdbeywyz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2jmhycovh.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2lqlftguf.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2xsrmiuyd.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2ctwqtgmb.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2yuelaukf.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2lupziops.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2uerxcgjy.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2kkakbyvb.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2bqxfqhan.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2wsavbzur.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2jwnrlyep.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2mrqvhvhl.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2tlufqmdf.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2zvwjsogp.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2lbgctefk.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mirlgamf.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2klptfgjo.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2suvnzjvr.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2foufqeqv.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2ohppnkpb.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2hpgkdacf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ouqvsnwy.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2vfajmtwf.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2hjrrigkn.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2ydfnyoqr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2lstmscrt.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2zesdgiul.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ngsperzf.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2wqnmlcye.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2pbeozvbb.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2nukeggta.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2qlpatxof.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2isgprisa.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2xluddkzr.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2ovejiqui.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2ncryzfgl.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2vjpdbufn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2pbcvnjir.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2yhnuhirt.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2mpsdfpxe.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2irxkiblq.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2eptmqzly.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2qwydywzo.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2wqsbmwvv.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2gimpifrj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2xnxstmkc.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2aehhsqjj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2odfxitua.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2jfhglife.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2zrdkxjsd.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xakqjjdk.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2pizimnqs.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2ozeielmx.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2fgydwgha.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2apzryngd.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2gduxpchh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2sjjzopqf.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2hkxtafss.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2dzsuroti.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2hjmjtxty.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2woyxoloj.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2ouhcfbsr.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2ogqnvrhm.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2dzcwakce.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2syvsidzg.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2ngsloqze.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qjtujibu.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2ulkimokx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2bfwaldit.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2ylesqidu.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2muaksunb.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2vicghvcg.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2xksrnolc.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2wfxapsuq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2kxxkaren.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2fumgewlh.html


<!-- 参考信息 -->