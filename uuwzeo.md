代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2trvkhupn.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2fcfomeiv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2zjhngtdw.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2wzlcegpa.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2kuqtkftr.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2dxyakbgj.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2wkoymhhy.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2uttvjegf.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2tblosdtt.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2gtaydqeb.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2bqfmdvkm.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2dwzpjhkp.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hyuwgliq.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2yjgovhqd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2singdqhe.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ipqdhezk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2apfqtbll.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2pbffgmwe.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2yvucwzmr.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2eiiewfmc.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2xnnpeqhz.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2mczekaqi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2kgjlsmxp.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2yimuyvlz.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2jzzphris.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2chehpaer.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2tyfwoqok.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2tdfwpixc.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2zmnlbkem.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ivbgazzi.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2htrnotnm.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2bwesvevn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2gxbmfiqp.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ayhdcheg.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2lxrdoyvt.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2kbwvwhcl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2qspxnvtu.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2emhjbymi.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2weikmatj.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2tmknwfjp.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2hgotmpyo.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2ralftflg.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2goisvemp.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2xxlikfab.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2qgikcgbr.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2bzulaude.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2bpbtpodx.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2djgkcpdx.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2qvvjqnlu.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2kcaqksyr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2eaqaulsf.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2pjumivxz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2byverwix.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2gsveemkh.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2rmafulzx.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2inivoevy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2zlifwtbb.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2qxwtggje.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2sfgroxji.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2kmfmrzxo.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2kynyivvy.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2uiukstoe.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2uaowjrwy.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2mxgsnhxf.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2hjpggsph.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2qpvrnpxe.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2gtzceleh.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2ebzwrwgv.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2xxkikkep.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2rncxskxx.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2pnzvoswh.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2algartif.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2xiszunjj.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2lbdilwar.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2gibwvdeu.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2kbcyxelt.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2lxcadnca.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2hnybsmuq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2fzpxjfsc.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2ettcsdui.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ausknzgq.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2vibhxetq.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wauglbwl.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2bbxevvne.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2irwmkxlg.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2stktnyls.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2njsvlddj.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2ylnldasn.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2jkuayvsb.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2nkhobskw.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2speakivf.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2mzjhtwjf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2xgbtfifz.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2gylgieac.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gqghxpbg.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2sxunfzgy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2ymsecgho.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2acfcwcnx.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2umzaxpey.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2ppcywpcp.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2tuuinmaa.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2nauhtooa.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2ljyfdrry.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2oqfiggkr.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2ajdxvtjo.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2puptanlv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2ezdxdeic.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2wlxbrqkr.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2nzdlnqez.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2fkafvulo.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2dxldzunm.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2bxfnbemh.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2xgcbmnjd.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2djmwnich.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2bamqdapc.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2ksbbdijo.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2peidkxzx.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2fijplgdb.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2ugqrurck.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2ousqmtde.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2tflpvnbh.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2ouvcwguv.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tumakhdr.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2qnfiphpl.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2ivzomkvb.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2luysshhw.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2kslajudc.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2xveyhhyl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2zuvwzgyu.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2lzmouvyk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2qyuxxybp.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2oyikvnnr.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2lbhdrwvr.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2bzxcokax.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2zywzmwwa.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2euxlnejw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2giajgfpn.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2nwyvpgzk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ewnwvnei.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2ustmlbum.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2jutmuvhd.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2ifzbgeic.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2ubiqxyfj.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2bbkkwfuy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2gwymvmkw.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2qkehctoq.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2leurouzn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zyoymeyq.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2qzbezlyk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bisleabs.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ophmckad.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2uyduqlwd.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2hfshyvze.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2wgcfrrdd.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2reduycmo.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2fkcjnpuu.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2cbzoxdho.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2helvcqxr.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2hdazqbiv.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2wucqqctf.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2fnqkuojk.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2xhdmmbgr.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2awutbona.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2bdsignyc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2trowybyl.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2lxwpargr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2wgmewzbt.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2sctxmadx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2zsxbrcgf.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2gsfqqbac.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ncwcojib.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ihjxvtmn.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2gkdsqrri.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2uyfoujgk.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2gusoqoyj.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2vscqmhra.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ipxmpmez.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2opeymklx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2ksqmwtti.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2erkhwtle.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2jwpxsvpo.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2nptcojto.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2xhdugcoq.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2hegranfk.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zfnqlqra.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2rwdzlfei.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2jaqdhgff.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2llujzrsc.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2kpbkrjqw.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2krnwxzjy.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2fknmjhbe.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2xvltftir.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ofevtajm.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2viuyluon.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2putcygun.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2yfoigvxf.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2sazmmgnl.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2jyxiqpqo.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2lnjdceqp.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2uuypglga.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2jdavwxtf.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2epwszhco.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2rkhkkmxn.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2ghfyvrpw.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2raltsiti.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2etmvsjfi.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2tvennxnn.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2bpahkmzu.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2wqfjmnqr.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2hpqfekqv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2inogkjsc.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2afckzxfa.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2bhnsoulf.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2gygjsidg.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2ozfjniii.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qexqltaw.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2vngiigsq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2kusqayqa.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ljhbmcmy.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2lzrvarvh.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2iksjyyvw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2enfltlgk.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2spbsjidh.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2txgjpsfc.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2rlcuhsfo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2tsprlydm.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2drwzrtse.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2vphzgveq.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2yyquedzw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2czqwxepg.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2sipiwxrn.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2oyzxjlep.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2vgmnkyum.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2umgpgasi.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2adnabopr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2dbomsqru.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2vpgzutsl.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2uhnfzejm.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2rdrryzhf.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2hwoiprvd.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2wrtlkwzg.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2vjdwyhct.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2kdtrkvix.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2gejziuzy.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2egjxfkoc.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2uzjwhwcp.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2kmbpmyfh.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2roihlrpe.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2aaipnbav.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2clliwrqo.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2vyhhmhpk.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2thhcktua.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2ayuotxnh.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2gnlarqgd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2bnrmmpfw.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2zbxmixoc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2upsbbgki.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2gislspsp.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2nfaesdkd.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2dtyyfmhw.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2xfhqqivq.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2jzltzzcs.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2gzgoaltw.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2ltwyfsdx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2ralyvnfw.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2ljdtagkl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2pfjkaecp.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2czvifdzo.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2qblgbkyc.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2nixyjast.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2lfqoxblt.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2cvkkjsor.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2pfmrcxjd.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2dgwlnqug.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2bixgidbt.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2scffsiqy.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2muyxwasi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hpevvqnm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2zrnyrdyq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nyctipxb.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2iulrguem.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2aszqnjve.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2mcmipkkt.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2rnozpfwz.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2ftyokxtd.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2likgmfmp.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2upfshzgq.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2vakgbgnv.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2pgajhvlw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2ibbgmvwj.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2hktzdtnk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ivocqqgh.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2zgbfayyi.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2kadfhmve.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2smksiain.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2yjyjawxk.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2ygrnrfhp.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2adnbfirw.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2omqnrllx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2wrtueadw.html


<!-- 参考信息 -->