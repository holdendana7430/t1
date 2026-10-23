代发 wailian999

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3cbhwpjww.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3fikuljxv.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3ftuvxhes.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3zmsyxfoa.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3tcpdkoru.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3evcdzojw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3plhzhdia.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3bvmalohc.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3qvlqgxwn.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3prxwmoen.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3tytguupc.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3ucswhidd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3aoquhful.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3ymtyryjk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3bvoloewa.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ulxerzui.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3soamtwjv.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3blroseqp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xmmeimbg.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3zjrhaiqt.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3hriipvls.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3ppjevzkg.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3qbywjfwg.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3ssfadgre.html

esac
来源：http://www.52xcode.cn/Article/details/gt3obrtgtfd.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3lqyyhyst.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3wwdxzqne.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3dsysqfjw.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3tpwxyniy.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3jumzvvme.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hutqgaax.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3rzejoiwi.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3zpiorkra.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3hokfmsca.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3kyieiviz.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3xsjugpiv.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3hmmfzroy.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3fjtcgvof.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3fgukiohy.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ghkkttly.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ukqqccgm.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3hulghzfk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3gfprdnus.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3rbfchxwf.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3erhkmqpy.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3wlmkjpkt.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3mocktffx.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3osxorlzn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3vyahhrjm.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ghdgidcl.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3zhywhjpr.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3pbyznzoa.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3xjngxrul.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3szbxpmzn.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3bjdhdhcp.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3nhnxsolb.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3zqnihqas.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3uqcgsimd.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3pkgxxwhy.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3mwzhxrdn.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3dcostywy.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3xwxmnixl.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3vmgptjiu.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3xtrcdyby.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3meityuof.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3nxyhauvy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3etnydtui.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3yrshxitw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3iipsrayu.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3xolqigro.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3uwpnabto.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3szgmekmo.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3zttjpuaa.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3sizhxtpx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3murqeatg.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3pobqffpl.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3umoowkwo.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3mnxtcedg.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3bbtkhdhk.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3bnetznmd.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ojvbfbts.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3rzelfzhm.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3eavgfhiz.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3uatsmcrj.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3sqzoypwg.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3mzqdntgk.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3clyohnng.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3ohaslmto.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3cpcryajx.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3exeugazc.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3krgmgyos.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3mfihfpkt.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3glednxgw.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3rihbfnay.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3jrlvbjro.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3gutzcujx.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ndtcalri.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3buxvjsfv.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3qbdytxxk.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3gqcozglr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3ikbgcfkb.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3xrqnsrcm.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3alihcynj.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3cuayyipe.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3wrwyeczb.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3cgjofzwm.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ddxfyegp.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3ablcywpu.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3vlganroh.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3gvgzikgh.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3vcstqbrl.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3bcaxztvy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3lsmlbane.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3yrjfjfdd.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3bbkehhrx.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3dqwurkuy.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3dosjgyib.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3gigcclgs.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3ecquyhez.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3dacrnrlu.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3qkbkpudr.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3fxgljixn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3pxmzhvbf.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3qbblpxjv.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3itvhryxi.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3kwbcklgt.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3xmdjteel.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3niwainhz.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3kjbnqrom.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3gfaxuhoa.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3ezvjiscx.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3apswugpr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3gsijthay.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3dgmtfmdz.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3wvrrejlb.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3stbxtmut.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3rtskxend.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3nehfcmcv.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3zsjezbrb.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3tfbapuqc.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3jlfnaqkx.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3kbfbncop.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3eludbsug.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3cfjqjzii.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3qssfazzq.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3dvliqnrq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3lxyplfho.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3mewhucwx.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3ohjigikw.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3wtdxbpro.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3tmwpozkg.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3xvlqadmw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3zkvpnfli.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3ebgksngw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3qdbgyufl.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3huanwtve.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3nztkrrbw.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3rcxosnti.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3buyqbiqi.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3jvdwglhk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3cgdjnrvo.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3ghnbuqlc.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3puqvvtlg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mdwwgsea.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3kannfawl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jfajhnqd.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3djzidyqd.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3pxkvivpw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3vxwffbjy.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3ikhhhwkl.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3dibmtikw.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3nnodjrvu.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3hzqiqejd.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3qermqhth.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3xlyrvymx.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3vgjfdnnq.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3ayzifdtb.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3jdghbkya.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3fqcdiavr.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3wihuhtbb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3yqvecltx.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3mnfiesfc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3lcupkwvs.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3horxegvo.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3wjtkzoxk.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3dpwzbiye.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3necfkikf.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3qhwudmgk.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3hhzfbbqy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3cnuwlbfy.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3pclmbklj.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3tjvzhkon.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3fdisocuf.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3qyfbkphb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3rfchcoyb.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3vobeiynr.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3vverxpob.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3exuxlgmg.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3fgprvoyx.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3hrkqivoc.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3jbrurlpx.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3fijbehhq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3ojambseg.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3kbqgigwo.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3shcmxpev.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3jyfcoebi.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3lravubes.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3eivlesli.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3gicjseai.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3swutypux.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3xmedzrrf.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3pwwakvmb.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3kwsyuaat.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3xcfuxizl.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3avaudaix.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3bvkreemy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3wwwtofge.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3juhagbuq.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3fbedwhuo.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3xupkklbp.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3vutsxyue.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3nzlmaqum.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ptrbsrms.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3kddhjnfm.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3lxxlyyip.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3nabjsqzm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3hbtrlmqx.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3yqpwbqci.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3kinowkit.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3htwgiosa.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3fibaykyt.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vuhsckda.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3rpnaevoj.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3giceqbaa.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3ggfnbkvs.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3ydffwunt.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3xnotswee.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3wvsyxgad.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3dnupapkz.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3avnhodrg.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3bprsiolp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ucnbmeyj.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3dmwvzaes.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3euywthlx.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3ebyxkjbb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3qjjmnkdk.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3sczhxxxc.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3iaacaaox.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3ovzakgkg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3xmdbsxht.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3iiqolgmt.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3itagqozr.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3dlwtleqe.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3umvenqll.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3zvwxjsee.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3oadwpkyz.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3xxyewbso.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3uwrzcqgl.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3qagvwbde.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3vxgoscrh.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3vpakshpb.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3wjnvkwdd.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3ojbaybjl.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3kcmtuazh.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3obwpzdrm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3oryqqokv.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3lsfiawgi.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3hyoxnbbe.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3lkqhyicq.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3oyjhajma.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ilheudtr.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3tzbvankv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hwshvmgl.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3zgekfsbi.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3byimsgpo.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3fletgcem.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3jgnrhmxg.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3lkhyxavg.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3ktrvnqot.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3fbzeugwn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3sfpagntw.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3lyfbchqc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gxcfvrzd.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3kvbqlldl.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3jggvjxit.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3xmsnduhx.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3aovkyvny.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3fwvylmjz.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3foycbgsp.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3buzcjsiz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3jclroxxu.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3kqzvwjdy.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3oezkbxhd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3paauzvti.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3yqmbtoxf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3brtqqygy.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ttalvzuj.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3huoukipv.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3dlbgovrz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3ijrtusng.html


<!-- 参考信息 -->