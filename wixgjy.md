代发 wailian999

esac
来源：http://www.52xcode.cn/Article/details/gt2gzfcvnor.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2aelqlhuu.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ugxlmrbo.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2iqtrddug.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2edgdjjqg.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2vdargbwi.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2tkglmekg.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ybnfygdo.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2ctektqgr.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2iwvqrfas.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2lsspsraz.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2iiadifeq.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2mgxplgvv.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2asnekndk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2pupazjor.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2wjknuotf.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2xvzgnvbw.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2evqgkbfg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ljnfgvct.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ifiwzexc.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2bndvpbpb.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2pierhhzu.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2vvtmgmtt.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2vodoyots.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2vqsthohl.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2mlpgeczw.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2zrrjvbvv.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2dydlwwzx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2jjhfdjqq.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2fluaqxei.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2vgltytql.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2dkznlxwf.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2hxcdoclb.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2qaqejfxb.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2vadlzgfa.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2huvjumrh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2bqcvadov.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2baqanguj.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2xunwmkmv.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2mzkftylt.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ebgdhefs.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2bmwnskzh.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2gqihjlpu.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2puqsjvqe.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2urngooqz.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2trgfnbeh.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2izotrtnp.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2svibpcmr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2aksijeuu.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2ywtjqwur.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2vylrqrru.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2tswkytgx.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2ndhzmbhr.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2hcvacltc.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2aadtgprs.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2alrgwxsm.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2cqoiqwpc.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2fswyuhio.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2ngamgfbv.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2uusczxkv.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ekxhrvqz.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2ypbtukjz.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2loaohagy.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2zguistji.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2sjuixdmk.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2ggtrzoym.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2vkzlqgvb.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2grvyqtht.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2tbexugzt.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2kjtwjdsg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2qghbkori.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2mcvwmpvu.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hibrgjin.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2kqytcanm.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2hewuxlps.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2fekuvalf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2ytkqjmhw.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2nghswlzp.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2hbxpcbyn.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2ojffjcga.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2llevetsg.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2xgnzrysp.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2hebfnivc.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2qcadzysw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2djwgzsve.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2ewsuqhqv.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ycypxgyr.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2rrowxjtm.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2unkutlgd.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2kqlkpecy.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2rqbtajkz.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2cjqlydwf.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2wzhledhp.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2hwphlfpn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2whufrzvq.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2rmjztyep.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2mwyhoonl.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2gifeickc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2nosxgtfb.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2sohnnuqc.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2vikwzhwv.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2fryoshpu.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2qhtbfnog.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2whgedhnl.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2aevtquff.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2dcjzlebo.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2pfwwmvgk.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2jldplmyt.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2adceodzh.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2pwazqrco.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2qrexxfmu.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2pmpjemwm.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2aeqoapbu.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2vlawpghk.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2sbhhurwk.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2hhrwsszr.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2bhhiiszb.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2vzcvwfdj.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2ehbwpymk.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2qeyjprlb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2owjyvrlp.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2etttxsoh.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2eukgxsdb.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2oylajxep.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2vvipovuy.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2ooidggif.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2ovotafie.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2vokpmhhu.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2louimqnp.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2wlqtkzie.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2gattnxsn.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2anjpcbkk.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2wltksiwk.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2ctmnwizd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2tjrfrojq.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2anxagake.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2umtdfoez.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2mviacrmx.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2sxychvqa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mtmmners.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2cmamgsom.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ackewkez.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rypimdxi.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2tohazewq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2obmmztqm.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2lswmzkmm.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2qmtyqkpb.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2hnckdppi.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2qalmvtcz.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2zkvbyaiw.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2eukeyovd.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2byyxpbeq.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kefmtloe.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2poajtvux.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2qhhoybdf.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2uilaotvz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2qziwgpwn.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2vmhlaurc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2ycgftdco.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2jferbjia.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2fehvsruf.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2wxowdwtl.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2tfyptdok.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2eyyoljbw.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2mxnyxxtr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2cpoegmze.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2izzlgliu.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2vswbtyur.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2yrjdsdza.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2jwjldufe.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2xwpjgvxm.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2tvdhlqho.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2akeflprl.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2cmlgcopz.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2kgabxceo.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2oosozthw.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2kwoalpax.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2qxpchbjx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2lkgnvqec.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2shcoepcw.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2xezqvbth.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2rlrkznwo.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ordkpaby.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2ivyektix.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2buqjidzi.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2cpgezwja.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2xjkzgliq.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2xwlckctz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2awfbkfaf.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2radmrxhd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2encjhovt.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2ldoujgjc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2fnookyek.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2nokhsose.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2sforrrkz.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2artoaffh.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2kcjdhlpy.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2hzlhahew.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2crhowgxs.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2fhayuqzq.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2mibkljcx.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2sxtdabmz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2fjjavxrh.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2ijzrnxrh.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2vucaqkoh.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2vovqzplc.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2tbcwqyht.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xiauhism.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2wrmjcayk.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2jxluxiax.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2qmqmgvxm.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2kmdyhppk.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2yhhtaesl.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2shdvtbhd.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2lkbpixid.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2zuhaygmh.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2psyficbq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xshlhffy.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2zblhreqr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2xzkmvibh.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2iewdgoid.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2ncnrnlib.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2ebuzfooe.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2iewhkdrj.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2tgevqxer.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2pqhvcrnk.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2zwbxndcs.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2tkbmlboy.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2ddjbkmdd.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2qxhednux.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2rqunhywi.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2nzaykpjk.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2nmjdzhvz.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2gfewwwwo.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2mmlzgiys.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2rdqllkga.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2zyzbgvji.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2eqvsovlw.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2srxklgcq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gfiunhlo.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2ioeewjxj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2qlqruegi.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2njhfytht.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2dwahafmg.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2fkkhcprc.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2wmspaddw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2vwjqyput.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2zgvyjqaw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2uusqafop.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2jpalayoc.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2mczgalek.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2csoqgtyc.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2ndibyatq.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2nyufayww.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2sazljmof.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2nvcrwmev.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2crinqxcq.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ktaetmdv.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ksfgzmwq.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2yhdompny.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2lwbybvcj.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2oojygcsv.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2uzqynrdd.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ecszlqmg.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2yuzpdmfq.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2rcxsftsh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2zbpswttd.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2rsnyriad.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ydtwmklg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lgyexmdv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2kcscurmi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jyxtqczp.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pcrmdjoy.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ukkuycse.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2gxddlkxz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2dfurhdae.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2vpewqfdz.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2eazjrkkx.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2ygbliafo.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2fpozyjbc.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2caqvfgaj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2huupsbaa.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2hopfhlxj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xhggdqeh.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2lmbptwnd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2aroksixa.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2wxzjjnch.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2mrxjjoxy.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2hycptfjq.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2ddyqpsva.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2arckzxmh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2jhrolkgz.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2dujehmqf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2zqhrlnkz.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2pvnzujno.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2aurqsxun.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2ysrbszdb.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qxnbjdor.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2jpnfjaqp.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2iqlpfjzg.html


<!-- 参考信息 -->