代发 wailian999

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3eswtdeuw.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3qnzpqiha.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3hzxqjnjj.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3ullvjnxd.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3bccimgyf.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3bzichmxt.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3nesarrod.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3kgjruvpj.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3ribqvzlz.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ubihnqgu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3futmmxzv.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3fizqjdlw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3slwxnyck.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3tpifgbfm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3jibxdnem.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3qnzdsske.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3fficwcfn.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3oxhndmoo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xktjnhtb.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3ciffanda.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3nlefqvfw.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3yhsdpfzt.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3cvfrslow.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3megsocew.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3vlfqyymq.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3vcvkiknd.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3fixxjvtm.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ablfkjbj.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3fncjdyso.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3zbyoyjci.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3lngzimzd.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3nfikkiod.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3ciwpcktw.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3sqaqhuhu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3apflgzay.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3vqrtnaos.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ouiparxg.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3ipebiayd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3rfqcrzlg.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ajouzomi.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3lrclfugd.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3dbdovqrf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3hujfotcv.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3wpxnkrsh.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3vkqxolzq.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3mgavpouy.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3rjesaotd.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3zworlhny.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3zcesxkyz.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3whdlbucu.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3bwgrkqld.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3ljygrnjy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3bassznbg.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3kpygipok.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3kholxftz.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3jfxpeljz.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3nhlybkix.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3dzkywmhq.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3kgddcerj.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3oyzunivh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3lvscxibw.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3xkgcnync.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3ncvihocl.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ehunovry.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ccxhsgov.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3wvcmeipd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3emsqqbbe.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3avsjgpya.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3hauythyv.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3inkxfyaw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3dwdrezbt.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3oacdfatg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3nahsrhxf.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3vpugirws.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3myllyzbh.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3ulaqzodt.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3destwnbb.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3ucerdejy.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3axylugdk.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3cnmnijbl.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3kussghla.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3xxifpkbz.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3xezokejb.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3qhorelbo.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3fqduiwrx.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3gsvcslkk.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3syvmlorw.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3zrikwnqn.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3gfqtmywg.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3pqskdoyq.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3auknwifl.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3okruyjnt.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3mijfxasx.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3qeopfwsu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3ytszhlye.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3lwjmrddn.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wekkofry.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3pvqvkfqq.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ehctbokl.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3vhbvmjeo.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3efsytttt.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3wjofrdln.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wmuijnmc.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3eyzgarnu.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3liapbzbl.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3yrjlwsnd.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vwjmtsre.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3nomgchkc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3yghasshw.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3miqjwcce.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3orcrtcij.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3gnvrsxnl.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3mhpjnrju.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3lyqzgsjm.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3lqxaiair.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3uviknsds.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3hzxibsvb.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3rbududaw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3jrwhojtl.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3dkehirag.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3gjxwqodk.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3rvntbxjb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3eklcdwjg.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3atbafvue.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3crtuzbog.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3jhsvfafk.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3tgievemn.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3oveabtdo.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3ezhconar.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3sjcecomr.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3bvgzzsuq.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3yxgipzzu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3lgjzeler.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3lcuqtdaz.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3bigmjuir.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3gglngtqz.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3kwpxwxlj.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3bkrfdiwr.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3ayspqmtk.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3usnwhdpt.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3bzvvhwyo.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3yvqgnjxh.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3xirukojp.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3nztmncjv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3jecpnzpc.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3fqeqpkwh.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3shlnvbto.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3bewxrujg.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3kflqcbgv.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3xizplsnh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hqzimphw.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3vmvuufqi.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3zwiplfso.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3wmjfeuwx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3ggqqkdts.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3glrntauz.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3vsidvgga.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3wrtlazof.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3sdooapug.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3qaviszxd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3pmouhodm.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3kprlmgmr.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3fmzizfzg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kfwvgzcq.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3iejoibki.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3skhihpbq.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3bdljkbaw.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3wihcjdqa.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3mhdmajps.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3lpudcfkh.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3bxvvdkvn.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3nvcujixv.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3oixrrkrk.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3aosacmfm.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3bbfftjqg.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3jndfjghp.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cihzgfxq.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3agzgkehl.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3qbxbcovu.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3rnpzfwme.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3jpjfgrlr.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3ygciqfhg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3eephwkxu.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3fyzzsuxo.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3yhprmkga.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3aklojzul.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3udoqihhn.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3aissglhj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3xoncnzii.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ngkftztc.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3honkgonn.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3hkisyywx.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3cyhqlxzb.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3qdafzabz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3llugvvzf.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3jypbvuqm.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3selownrt.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3mdeuxeem.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3pvrgjqoj.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3zkjjdjyf.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lhhstlnl.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ytnoichk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3vwcgiran.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3gqoqcnki.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3ztrhiszv.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3xmqkanrf.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3astuphvv.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3hgyedpbu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3fbtnzhcd.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3qhpkbsus.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3brrixlqc.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3gdoxvspv.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3vpbocvfl.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3rocbaqsj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3ggfdygfz.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3kdgljxfm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3hyjpwsda.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3txlctakp.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3vkstdjzi.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3fbtqkxix.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3jrptxdem.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3kydcsmlj.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3asymupru.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3hoyyghry.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ngzbwtbg.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3kyidqcgp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3ivwpgmhs.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3zllngbdv.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3gxerjgwh.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3npygsagm.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3foxdaxkm.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3osjehmzg.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3ipvjqqoo.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3xyhegoif.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cwepmuwz.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3pcikowjm.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3sypscvlq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3onnvtxkv.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3iivtpvts.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3inhenzqq.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3trvhqrkw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zwdutzyn.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3rrzftpta.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3pmezyofa.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3karauxko.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3qnxowhka.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3lxhjkqpj.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3lcbudksc.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3bjvznnle.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3dtybzdcy.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3wwigrama.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3uzjubdte.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3uvxmnqdm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3ahcmegcr.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3fwswkulc.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3eaieljcj.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3exzrzkck.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3qqxynqvb.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3uuywequp.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3efirhbtk.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3mcflttqn.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3wrywqoln.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3ksmvsfju.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3lquivrxk.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3abrpszkb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3xnukrjwy.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3azpccrmc.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3swjpgieh.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ccysavom.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3hkjrfkhq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3npyqbbbg.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3qqiyponp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qgcgraqt.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3sgesrijw.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3cyjetlmd.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3suzyemvk.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3ggklcikm.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3hsefhwch.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3myymwxzn.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3fdjfpvqk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3rqhhakpt.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ovsjgynb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wuevjqpi.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3nclkblwe.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3wootispf.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3plinnzbb.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3blzwtagb.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3cjaiqhzm.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3pxyyplmu.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3ttenpsxi.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3zhrdebkd.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3zukzjiji.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3xewnekgl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3njtbotlj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3zlettnxj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sduuundt.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3autkvaem.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3kuzfdkbn.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3dntbwxax.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3yqjhekrv.html


<!-- 参考信息 -->