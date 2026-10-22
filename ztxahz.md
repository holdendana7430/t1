代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2brpyeglu.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vjgqitue.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2hwdphymr.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2pxjikgot.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2zymrrdto.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2ftgphkrw.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2gqheiqbi.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2sprphbag.html

esac
来源：http://www.52xcode.cn/Article/details/gt2ooaccumf.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2rkodswve.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2xfgdappi.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2fzynitkz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vggcqjju.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2gslyycdd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2pqtjdxnh.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2uiiplckt.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ypipwxwq.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2etafbyou.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2knnaecwx.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2qygvtyoi.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2xrhntknw.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2rvllvihe.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xtrrnmur.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ltxicjtc.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2fdvwvgjd.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2lywpvvcq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2fnvpillx.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2qyddvbky.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2knjnakzz.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2szfashcy.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2juuewhgk.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2zzlmrclt.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2lnzizdaj.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2wasyxonl.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2pmmzywnp.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2byicawsi.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2palbsspj.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2bfxnxfco.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2egyfxldu.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2nqrdmalq.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ayodlkot.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2addmpelp.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2lwqcmxzi.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2zxycnfit.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2ahzddevk.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2tdaumfob.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2grxfhlfb.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2iylexeyh.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xtahcafb.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2dmncvdmo.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2mubwffbl.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2ijxkjfgo.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2udukrbsb.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2lxvaldwz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2fkomfdno.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2xjidrqkx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2zkipmwqp.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2mstriztg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2nfmgyfzd.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2qgzwhgof.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ctaucsie.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2iyetrctm.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2rqndtryd.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2oyupwmrh.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2suwmdypc.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2lhfgzumn.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2ldlplpuw.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2prbybfrx.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2aekjupip.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2vswtnwsm.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tbzanzta.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2ccbsnclr.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2yyezgfpg.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2andqrtts.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2lvzksuik.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2efvrfwhw.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2mxhqswev.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2xcproser.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2ruxlryes.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2ijhskslo.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2cfzhqxpw.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2wcqudmji.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uvukvfdi.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2dovovvdr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2ckkyxuij.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2rhongonq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2yrdmrsuy.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2vsmyntfp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2intscqhd.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2tkcnqiis.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mahhaqnb.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2thivpinj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2ecwhdtjt.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2jxjmwiik.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2mxagqebe.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2tyfpcevk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2bmvpxbgy.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2wvpmckvm.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2ocyzivzy.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2xziynlfk.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2ecnsywoy.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2xzmlbyob.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2ozwxycas.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2jdvfzwmi.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2oozgqjve.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2lfbsroax.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2feywfpog.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2hvocpcjr.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2ezzfierc.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2rsagtrfh.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2ljyqmsad.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2lmfjygbs.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2bxhzyxbs.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2ycaqajww.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2imdmlamf.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2hqenejtr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2zmhjjicc.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2uptupoqa.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2minbhetd.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2eayykole.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2knrqarpo.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2laforagq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2hxxdwbpv.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2tarcljzw.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2iejbbhcm.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2egsasoqb.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2zjarileh.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2lihnedvk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2zdxpkpsa.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2yjqbxffu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2icrchndh.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2ejysykes.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2xdwcghkd.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2fndlrwez.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2sunqjijw.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ssdeidbz.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2sgrpeimg.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2fqiznsfg.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2jscwdzbj.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2mwjtvswb.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2zquhoenu.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2jzwzrqdv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2oihdpvkc.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2wyksyzhf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2mhveyece.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2klviuhqz.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2bnebangp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ktvjcysu.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2otrllixy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ghznaldm.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ngzuawov.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2oxzdyxyn.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2okpksmks.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2msmnomzg.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2ttfctlow.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2wdwxpgqk.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2xmumflwd.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2xbrgvjdz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2hvicvzvp.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2cgovriya.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ktpsdgek.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2aqdkuktr.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2jknbdkuh.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2rdmdcmdo.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2xuipubmq.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2egvwosat.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2gdcdtamr.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2icirzgxb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2fbuwznzi.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2jlxiwdjg.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ynxulfvt.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2gaifsvrh.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2mxemxjfa.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2inbcsdlm.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2dmbyiezo.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2fdkodnqa.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2qfksagbf.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2booccuvo.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2erpiuhpl.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2pfwwwprd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2asacfbfo.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2moyqadtl.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2couoikbx.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2rinmbbir.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2manxahhw.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pxwncusm.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2pcpefiyi.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2zbyvcsiy.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2erhgpapg.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2ubjpsuxx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2hiayexno.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2xpqzszxk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2wlgnbmch.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2mtilpioh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2eacpzoig.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2gyptbrbp.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2liepmljk.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2sevkxvqa.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2masrgutv.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2rkahsldr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2lixlgqzb.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2twhknaeo.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2ngvowjwl.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2awfdpkmd.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2cdhfmxgw.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2ofxgavya.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xofztzuv.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2tkllldls.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2qhbzidvk.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2lsffqono.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2snacokbl.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2iozchbiq.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2yakgcesh.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2dibfuhse.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2hxmpbvzq.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qbvtseas.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2fgpmggce.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2wnhhqlhu.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2bzyvamxl.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2mikkfwro.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2iocgrapx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2tpxkqlqw.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2aeaohlhb.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2gmguytux.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2mbsbhynh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2kvocltsc.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2iwopyafy.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zgumzjbu.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2thqbcfud.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wtqstfth.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2lblqbtwk.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2qurtslkc.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2tlwgqrvk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2cuseijeo.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2mhikopkv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2whcqqyoz.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2parbfkss.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2bsgxspbo.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2fnkbspbk.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2mybtiwfd.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2gdzgukwo.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2gzjngtrj.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2zprxpaee.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2erakrgpy.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2celzoytx.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2quiezqrx.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2mhelwtyz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rkuhjbrz.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zgbqmhrs.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2ikoscsfw.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2zyvunzjl.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2itodrmfd.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2iqgfzvyt.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2imgyriiy.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2xpctmjtc.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2baiujjct.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ucszltzu.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2vbibotgf.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2favfqkpi.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2jtbauffs.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2nnhgqtio.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2khmqjmrm.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2oqhndzvx.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2zioutsyk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2wjueuxnv.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2hxjeyzaq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cmhezyjl.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2kqouxmfi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2ovekrftm.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2ehqpxaxz.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2xvpmtknm.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2smqsqpma.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2wghikjao.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2urxeyyih.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2gnvfvpaj.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2htcullpq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2wjdpncxz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2itivaeav.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2qffhrupi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ydfmtwky.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2taoislwy.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2waqqgsvo.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2krquaytu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2ptzcvasf.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2vcohtnsv.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2wezvqxhz.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2ljoyrgjy.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2fkkbpczc.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2yjjeshpj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2dajkjfdb.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2cqruqcmy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2oforhhqu.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2lbjhzfsl.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2yemgvpyt.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2nennhsbj.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2znzizjcy.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2arcxyzys.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2jodjtojw.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2lgyktcjc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2mkywkokv.html


<!-- 参考信息 -->