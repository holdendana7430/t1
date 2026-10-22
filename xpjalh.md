代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2oghrusnu.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2orvunyeh.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2jxtjoxzh.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2rbsvnyio.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2kabggfqp.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2knhyolyv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2montwdqs.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2xjaguhst.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2ngucmoon.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2opbpytqp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2vudffxji.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2zfcdawrs.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2eajtvqxd.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ywxbkamw.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2gmztxslw.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2nnxofcqq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2zjhceluf.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2pvskapsl.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2tiizsmkr.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2pshiazpl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2fcwderck.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2nawfiiaw.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2qjoefejy.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2ymubascp.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2edwwlmfn.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2eeqvcxhw.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2qmruegii.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2tsffhlpd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2xnwjykay.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2jziotteu.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2xnneggrj.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2eziroypo.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2mtpwlozt.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2esooedub.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2bfcdbkni.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2ycgmjliv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2ckupffby.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2skgadovm.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2hgmhcqco.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2acflxjao.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2xuvbgjzq.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2wnixbpbw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2hslvesxr.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2caefejfo.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2npqkqirq.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2wljlbtpw.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2uonggnqp.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2vlfsviah.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2qfcmvxlu.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2lmcizxfw.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2bgolclks.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2exmqkjbz.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2tlxqpkug.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2dhdyvgsh.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2otnlyhtm.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2fnnmeewj.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2jhtfphbv.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2mzmjyqbm.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2qtcquwma.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2tlrvtdiq.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2omkejfft.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2pcureuvl.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2mnqfzvve.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2wzatrihl.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2lpoeawow.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2olrnfvpd.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lawvztch.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2qpwtaome.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2pfsmyevc.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2ncofasih.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2npiaiyet.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2ietrvjnt.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2tqrcktal.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2kgpsjvid.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yfraacqb.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2itigrobh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2hpodzuzy.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2jeshxapr.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2uanqgqbc.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2byzzytaj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2zmwevyiz.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2saknkfnm.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2caerfpcm.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2sbylktgd.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2brhlufhb.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2tjcumgoi.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2bpvdgyom.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2muonaqsu.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2omomtokb.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2gfghyujq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2ieyudojj.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2neugumdn.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2tkumbxaz.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2aymxmrle.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2yombmmch.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2fndijaqh.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2fdvwmuja.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2mlccekwn.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2jwgipyep.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2yooruqum.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2edczotin.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2yxfgydlc.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2ofkplxgs.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2rtxliohd.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2issngabb.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2crftxpjk.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2crqpdwtl.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2hzbplizp.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2oikihbda.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2hnxmuxty.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2wlgkaogk.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2xhstmlon.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2stuhcojw.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2ibkuwhzr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2vdghlzha.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2zikfwyll.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2bggwyrfp.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2wxjzyhwm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2wlcsmbdw.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2flptoupz.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2nsnafoie.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2btfhvgkg.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2vdtkitbo.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2yxqwdxhr.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2akqhszvf.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2zbfgcszp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2pqxvvahm.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2aptbbubj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2dkglcctj.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2qjrsybwu.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2trabecfl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xwvqisik.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2auyvuasz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cctaojeo.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2trqgekdl.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2onekfhct.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2lvozuefh.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2bqinhsux.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2ldpwevny.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2ruorblgo.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2zxkusoeh.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2zlbcfnjv.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2weikwadx.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2vzfwkkif.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2nmuunhdl.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2dnvjeyhp.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2mgokpnvk.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2lqyxapzp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2lyogjylg.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2vtowsydh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2gddxfecr.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2gjjnwzgd.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2ocorpqkf.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2rhxyduvo.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2asiwbrgh.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2siktjgie.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2hqnrtvwt.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2rgjxhkin.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2fzfxremh.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2muwoyxzm.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2stsnwaqo.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2fpduzkgm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2bfvpvfms.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2oufiwhst.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2ggfciahx.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2zfkvzhyn.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2pztsydna.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2bnovxaqc.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2pybypsyf.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2miclvtbl.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2okmidpyx.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2umejmoxz.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2ofuqrvgw.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2ohsbbewk.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ixlslerb.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2cojvzitk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2mnejwbfn.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2nawwnylg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2byqjsnyq.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2tmdhdueo.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2swfrqwhy.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2hsejtstd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2jhejodlx.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2vxdqcngo.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2psjyioal.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2yjuxpwot.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2uiaraoji.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2qgutkrrx.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2xfguthvw.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2llawrksp.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2hnpnzkge.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2uzpgqkzj.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2gwqkqncp.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2roxjliiz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2wskqpzcf.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2mnoligba.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2lhblixjx.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2suntllan.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2sdwvkdvz.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xgulrclb.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2okfyuczl.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dknfggvw.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2nhcojtyk.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2hskmbbeq.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2hzxjobuq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2odpuwbtc.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2lioanxuh.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2xnwetbdi.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2pthsqnlk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rgiyvtut.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2uhraujzh.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gfgxmnyf.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2muqzczxo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2ynmrpbee.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2bugyinlj.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ymtbzptf.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2tjtwwhok.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2jebqkdsq.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2jbdnobgh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jgvhrpgk.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2kksoeyhc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2faluxect.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2ntwszzsz.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2sctobvpa.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2edlkrgzk.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2tykhsvsx.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2decdhdbn.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2vhnecnvt.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2gucwtltj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2lhduwysc.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2lkohzwtr.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wyrszetq.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2hxewdpdn.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2mzdkbcgn.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2hlpsclgi.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2pbdlweoe.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2isobcznc.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2bwtuvlpi.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2zrjncdky.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2xodyvcnl.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2cdduznta.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2arsblmgw.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2tukzvqvh.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2aopofsgt.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2lmsuugjt.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2vbildnnl.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2bbnliakq.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2frqdsoug.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2cpdrboeu.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2xcfnzcou.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kftidvng.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2lytcapnk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2ztlbbnts.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2faycixws.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2uzfilrib.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2xdnrlqqd.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2ruvsbovs.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2lyvurang.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2lngjdjhk.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ogzmmzrs.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2uitszqou.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mnxcdfuz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2sxofwkly.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2suaztxqp.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bqqxaqhm.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2xxdlkper.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2rhmquzeq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2fvvpmurm.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2ztrraser.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ewnqdldt.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2jqsgtqlk.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2tiysvcqm.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2ivcxqwjc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2vavdvpnt.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2hkobedsn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2mlfindjl.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2mxfjuhzc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2onrcqzio.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2zgfzpqtc.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2nyuyuxhv.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2yczbxpvw.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2nokalbfi.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2vwkuvaxe.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2bkxgzesd.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2pzvufjqe.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2ahztpqtj.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2snjsqvms.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ubllynea.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2aukttkav.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2orznvxhe.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2legeytfu.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2egpihpkq.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2kawgiqbu.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2sodojpfx.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pftwcvid.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2gutlxase.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2vstumhja.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2vgyrvxzp.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2vikcaxka.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2zckvwonb.html


<!-- 参考信息 -->