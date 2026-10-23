代发 wailian999

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3wgxhodlq.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3nmicubjo.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3yxepduhl.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3ihzncjdi.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3vgntqaxg.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3tpftpfdj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3qwqbqcgd.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3gwlsadod.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3gpcndetf.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3psdjkcax.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3uzuuhran.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3cwlmnsup.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3zeplbwxu.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3tdlbnphm.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3khmhqses.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3wxgwyffs.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3xlufwucl.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3nhczccmj.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3wdpgppuf.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3nqfakugj.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3klvbastb.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3awmmhesc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3rzjdzzdg.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3odgpwykf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3fubspzvp.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3iekyxmrz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ftvreoxk.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3xxxusvua.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ybuevnog.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3vphgojcc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3vibczsip.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3aztllvgz.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3eewfypqu.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3gdzusclh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3tzqmqrbo.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3qrnarmdn.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3jfjdqgcj.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3eglkktzd.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3ccjivmib.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3adgmiqtc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3bhlqdlkc.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3kbfckshn.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3olizrolp.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3kaopqvlz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3cwklsfkg.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3htkalcgr.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3grpmhwaq.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3xiipzofn.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ocehjphk.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3zcyyjrpn.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3tevwiwpg.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3enbhtfre.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3ootjxija.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3kyvtezkw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3ccjjhaqk.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3qfvvfyxg.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3nhohyurq.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3zjptxpro.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3dgfgerdl.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3vnnnzgmu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3zvravarf.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3qhhzzveo.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3qbbyaflw.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3havgnryi.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3gnlaevmr.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3omhnpwld.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3wrgsmcha.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3kosbeguw.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3sltsgykh.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3vgaeliyw.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3bozuusgo.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3fuuzbemy.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3dzvluksw.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3pgiepzqf.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3igntckoh.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3oclptqbv.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3zluoyzkt.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3dehyfgjh.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3eqgutuuy.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3bxqnsqhh.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3kzukncne.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3zgolouxu.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3uuoghuje.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3bamdoiqx.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3manpmjzx.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3blgrhzdc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3xotdohdt.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3xhzvkomm.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3iacxdsem.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3crxozjlb.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jkdcdkol.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3sddnlxbh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3cjjvadmq.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3uuqjlgcj.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ybtsonio.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3pxqzodxb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3kjijoskx.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3svrayqtp.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cqvgjczl.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3xrmladee.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3mpfpvxdb.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3pgdevtlr.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3btklqqvh.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3xdiupwxk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3gpddcotp.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3qfdncouu.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3nurzqmal.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3ksbxeuaj.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3ediuaqig.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3wjikekom.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3qdedfdcm.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3jmgoench.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3pscexbmo.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3puevfjqo.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3efvyopgy.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3aljhfern.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3udzosjdl.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3fmeybfae.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3pnbiizww.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3lkaqvcra.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3jhdgawhd.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3ojrsspru.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3iitlpcfc.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3rzixcaio.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3ubomxwgr.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3oisbabpv.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3wpkqizzn.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3zblwmddx.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3rydyiozv.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3uiiplnpo.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uvemoxts.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3cbizclbh.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3pzwfvymi.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3bbunciij.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3wrlkspmn.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3tdbvmcbz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3vojpcdxc.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3bqdjttqc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3eztcdkwf.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3mydnmozx.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3hytcdjhg.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3gjdkocbm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3mprdteft.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3dmldzxex.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3iqdxjtva.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3ghiplrth.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3rcmbnowp.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3iaoozsce.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3aggqmbnm.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3minzxvah.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3lnpkvlqh.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3gyvagfcv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3fdrvcptj.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3qyfymbdf.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3aptfwdvv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ngcmjrhv.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3wnwpurcx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vgrkaxay.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mkmqeqhb.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3xmjcegse.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3rprtnwfm.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3jrvfhrcy.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3aoxxrfhj.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3qcklfzfs.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3eqiyqywl.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3cbkcxyvh.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3aealyhgj.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3mdwsbqyd.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3muhcfmdf.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3qaasqoov.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3hfgaimim.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3yolnnhsl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3mhftauvr.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3ukupivwq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3xrhugnxo.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3xzcuuwjj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3tfpijtsn.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3ujqgubrl.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3vszccapt.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3rbpbeint.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3khubatld.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3unhjztan.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3favjgkqh.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ejqvzzfd.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3hedsjdpg.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3izcytqok.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3aeobhfpf.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3fxibnsjp.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3krimupto.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3rbyylkwc.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3vlonejrz.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3sfagtgid.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3fsyxyebw.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dfhchtkj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3pmiubzfg.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3houpuafe.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3zbkiciiw.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3mpmqgkpc.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3hfzxrydr.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3bccumxws.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3nglwtosj.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3qbktqgoa.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3ledyljha.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ltmylagm.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3qarkjaua.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3tmwwopkj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3uvrbsyun.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3pzjolfyk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3ppuoyivs.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3gkhnrcxg.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3woegcxxf.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3labhecgg.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3ozqdifxd.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3wxuhttfu.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jkqcdcot.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3jhnyjkjy.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ygkunoej.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3lmvcbguf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3jhnkoomp.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3gjucfgvo.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3gfrrnwcl.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3xwundvux.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3nqxqzqxd.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hjqwpsxi.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3ympmcjgs.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iuhibjcm.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3opmmzxxd.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3ttcysfus.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3juachthg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ibhqefpf.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3jvmbmjzz.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ltubeqpj.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3lmdpegjd.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pzuvptuw.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3hblokzgz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ajxjrexk.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3lqcpqjci.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jovizpqz.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3losfqxar.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3rkgaupwt.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3cbdtgewa.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3vxoktjgz.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3vstprbyj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lsvgnkvj.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ptnctmxx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3shijxifj.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3ducmbcok.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3jomklpqp.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3cpbhfvhd.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3hidpsrxq.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3pjnbxnyw.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3dtntpujv.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3zqjlfbue.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3qxsyglvn.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3xqvjyelk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3uvvrmzbw.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3jcycniky.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3fxctxczh.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ykethgef.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3yzkkdwfa.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3muaruxle.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3rfmfmnbi.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3ptjolmot.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3oaxoqdsq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3mhhqfafv.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3edavbqmw.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3fscknabe.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3wqqmdxuj.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3xxpsudtr.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3xdhofcdz.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3qzaurlal.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3zgnbpjdj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3bhntrgso.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3qiqrsipm.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3qeknluys.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3icuvoewl.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3cdaqtjmt.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3ptmuvwvi.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3tnitvsxb.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3afxskwkq.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3lzyympqy.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3bgocltnj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3fzwavbzc.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3rzkrastl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3mnvduhbd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3elndjdxb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3llgxwsmm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ovpedrwr.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mdkvfgqr.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3kgbpftut.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3jfoytffw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3uousplss.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3nzrjgkts.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3mrxoawtp.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3picmphqu.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3eenpljyx.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jscyturt.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3jbvlurys.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3tglbfpvx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3fwrlsafu.html


<!-- 参考信息 -->