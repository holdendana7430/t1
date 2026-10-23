代发 wailian999

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3cmpfwsuy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oysuydpg.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3olazcyrp.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3sitzrijn.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3jfzkriys.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3pwrkdfgr.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3ankldija.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3thnayhyc.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3ocnjbgsx.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3dfyognkx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3ilbmftxr.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3veyxkajt.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3pfozvric.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3qlsbtlea.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3pkhmeice.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3ycbaayoo.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3xtwwltfn.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3brngjsqz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3vlvxkore.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3jyizqoow.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3sswqqffz.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3kpkuufhv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3ujvkroef.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3ixrxdrtq.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3glyrbgmr.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3oxnwtqcd.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3gayknaar.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3rettubel.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3xaqkuitg.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3novoighp.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3oeshrckm.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3vstqqiee.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3tgsohqwo.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3angghknh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3fjbxwuqo.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3yygbevvj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3zpswguls.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3qhzetumr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3zedmwsfu.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3xgfezeth.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ujodoakp.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3pwzdinuv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3dbhqoxdp.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3wtfudxss.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3thngfwqt.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3flfoqmyo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3boovsyej.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3pgbsqipr.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3iimmivxk.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3osbxaado.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3eccukumq.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3uwnutxtr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3iziqjxei.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3oimrfzvg.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3bauoiuaq.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3ljiisqbn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3adyssrik.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3dvnlsmga.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3ecmibmxt.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3lcqebjwt.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3hwjzyfre.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3hkwcksdz.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3fgzbcgzo.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3vguhljvp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3tfqvuyrk.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3yxcqjzpy.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3skfdwbbi.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3dyebtpxy.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sdezltkq.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3wwnosxtz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3iwjzsknu.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3chuezszb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3muubutda.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3mkdgxfoo.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3yxdmumtd.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3rudysmtn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3fdubcoqe.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3pfsqlqcp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3cophtmfj.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3lwhbzkdj.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3uahgizgk.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3wlmnhyzk.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3ehtecggr.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3lcnhtelh.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3zgadwwcn.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3xeumxksx.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3llpzfvyt.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3omjpeavx.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3trhnzmit.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3wnfpabqt.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3cdhvqnnu.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3xiwzohgj.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3svjhawqq.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3hrrjmgov.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3rumabwbd.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3pgalpxwx.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3bnuavjmy.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3kirlemay.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3fjefptvw.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3uowsxumi.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bemqxcjt.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3ogwwukki.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3tviyjguj.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3jaaelyzm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3vhywyacd.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3mgnnyqkh.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3vsvjvcrw.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3blvhhhte.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3cveikktt.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3ogeaiava.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3xvnpkjbj.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3pqhwxshf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3wxfnshve.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3wqgraktm.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xldkmqtk.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3slcflcwb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3gvggufbm.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3hqjvqarw.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3kidynrxa.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3udqxbvtu.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3rnjvyjjv.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3tiixluok.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3rwgafusw.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3nyntrnkq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3curudmez.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3wjfsbofs.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3oluumnjv.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3wrpwwaiu.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3qhleeljm.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3bfmacjwa.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3wgoarlwo.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3wzeshnpr.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3nkugituy.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3wngtrkpl.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3agqdjeio.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3xayhjdrz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3ofbrqjzb.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3vweuneih.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3xeilskyr.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3etnfotmj.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3xjlmiaer.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3defyyrnb.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dvsmjiwj.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3ztztdodu.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3ergxgsnu.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3zeanamva.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3bttfdpwz.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mufqdgsu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3pntnjaqx.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3bohmszks.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3aakxykbw.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3iarozjat.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3enbtfxae.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3iycgrnha.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3nqciujox.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3unyjnaph.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3tpbxqwly.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3htucvedc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3xjmepfdv.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3ciykbwjg.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3aqowloru.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3lparlhvp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3uziqxybb.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3pqxcgkkr.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3nmsciisu.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3bvlrnrag.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3jwkzkzau.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3svpxnond.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3osajhoxb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mfqkoazz.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pbcbxefc.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3cwsulbtg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3nfcswgnf.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3zcqlanmy.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3trhirycz.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3qaoesime.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3enrjqexr.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3eececvse.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ghzehrke.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ovkiwkey.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3manmtwwe.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3blhncicw.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3bmthtehk.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3rgrtorid.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3szmobfol.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3hkzvowsn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3garyjjnw.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3vrbryaro.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3dntaysum.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3cejdscqr.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3xytamkss.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3hujthqrd.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3jyiskgcj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3xobswiqw.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3llmnaofi.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3qcmveqkn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3smnnaoor.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3balqezqm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3rmxneqnq.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3ojuboekp.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3yewxepwg.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3ontvznfq.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3bshtxbzu.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3qoyroalt.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3luqquksy.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ajrkaezu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3kdgkhjnd.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3nyqshhxh.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3kcybjyiq.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3nlregdxa.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3yixqgeos.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3hfmjxjtt.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3tgvckbfc.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3ddgoahys.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3aeniimdh.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3unhtttps.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3jkykdeir.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3hgzvdotm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3golclndn.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3fmyqbfdv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3soavkyca.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3cazfahxm.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3xcbantpf.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3mbndanaw.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3enycuuxl.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3szijjcro.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3iebvwvmj.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3hwimlfoq.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3maxggtne.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3wfxcpagf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3bwjkuaka.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3mogdcrbn.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3naggqnbe.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3orkbyvqq.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3ogfktvwp.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zyuxnsyu.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3awvcujxa.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3makbbsah.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hswpcner.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3vskpztqy.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3siqmtfvt.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3lkokkdyi.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3csbmhrrq.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3zdauadcp.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3rzezviwx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zzcetscd.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3tmywqsfn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ulyirqqs.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3aedofzlw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3jzbfwzxj.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3pfpyylhc.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3fhdsntss.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3jpmnqhsh.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3xtrphmvb.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3wnspqwap.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3ogtryhdn.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3fzkjokhu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3dxlehcul.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3upbregkj.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3zpwjyxnm.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3kclbbyrs.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3bxnhdwmv.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3oxvsaoqj.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3jmnhbuzy.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3yzniuxlo.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3cpmjzsln.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3dhylrmbv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hropjjno.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bduukxam.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3ttxszcxm.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3jfcqhzny.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3ehgbzija.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3wpofunbb.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3zcuziblj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3zpysnipt.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3vdrnzjnx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3mwjflkai.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3txuevppy.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3dcetdnbd.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3dupevpuc.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3wxbknlvx.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3vqzhvjko.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3rteyplgm.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3dmkqaprq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3xrrxfdtj.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3yobuafzc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dfrgjexn.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3rsyloiiv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3gvxodfjp.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3pqfqugwd.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3fregzedo.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3iskqxkcp.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fzxjppfi.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3ndlugamf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3hawcigfq.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3ycyjhcrq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3hahnzvac.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eerodtfc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3rrjqcyng.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3odjefhao.html


<!-- 参考信息 -->