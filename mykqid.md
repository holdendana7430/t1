代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.sweek.top/gtvvyrdawy.html

[R10] 正则匹配
来源：http://hz.meibo888.top/gtzftjrzmz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.daxiang520.top/gtleatvrxq.html

[R11] case 多分支
来源：http://hz.316326.xyz/gtsuycllhm.html

case "$1" in
来源：http://hz.wangshuangyany.cn/gtjugushmc.html

start) echo "启动" ;;
来源：http://hz.jlsjyb.cn/gttutchihh.html

stop)  echo "停止" ;;
来源：http://hz.ybcxt.top/gtosmvinbk.html

*)     echo "未知命令" ;;
来源：http://hz.jianghu66.top/gtfajjzybq.html

esac
来源：http://hz.jqgfzy.top/gthnhrjcwb.html

[R12] for 遍历文件
来源：http://hz.yuanzhike.top/gtwdxujvfy.html

for f in *.txt; do echo "$f"; done
来源：http://hz.tianlin.xyz/gtffbfsblf.html

[R13] for 计数循环
来源：http://hz.snrcjt.cn/gtjdahhcxb.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jqgufenzy.top/gtdghmufgf.html

[R14] C 风格 for
来源：http://hz.jqgufenzy.top/gtkrewurir.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jinghuilouyu.cn/gtxmqhhcrc.html

[R15] while 逐行读文件
来源：http://hz.hysaishi.cn/gtkldbeaub.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.xuanzx.com/gtispyrrak.html

[R16] until 等待条件
来源：http://hz.zhaomingkeji.xyz/gtqrkhopbm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.zhixingplan.top/gtchrngcgo.html

[R17] 数组定义与取值
来源：http://hz.shanyushiyangkeji.top/gtssqeyuqq.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.bjfxy.top/gtfiwunlvt.html

[R18] 遍历数组
来源：http://hz.dianchejie.cn/gtaetkknbs.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jqgufenzy.top/gtkhwktgjw.html

[R19] 数组长度
来源：http://hz.xuanzx.com/gtfhhewcsx.html

echo "${#arr[@]}"
来源：http://hz.gaohongyu789.top/gtsyfecebm.html

[R20] 关联数组（字典）
来源：http://hz.cheryme.top/gtttlqsnfl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yj20258.top/gtmuoolsbw.html

[R21] 字符串长度
来源：http://hz.sweek.top/gtsabghdev.html

echo "${#s}"
来源：http://hz.yj202588.top/gtftuehqwh.html

[R22] 截取子串
来源：http://hz.hnxiangtu.top/gtlxwuesbb.html

echo "${s:0:5}"
来源：http://hz.fengsongda.top/gtdrffegsg.html

[R23] 字符串替换
来源：http://hz.shanyushiyangtech.top/gtgjluluze.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.yuxming.cn/gtrinkwiwa.html

[R24] 大小写转换
来源：http://hz.yuxming.cn/gtidbeuoua.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.haohaochexian.top/gthpvimebd.html

[R25] 去后缀 / 去前缀
来源：http://hz.jianghu66.top/gtbovgitpy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.zhixingplan.top/gtxmuvbqjw.html

[R26] 命令替换
来源：http://hz.pycfn.com/gtkhfsnknc.html

now=$(date +%F); echo "$now"
来源：http://hz.jinghuilouyu.cn/gtvczlxgbo.html

[R27] 算术展开
来源：http://hz.tianlin.xyz/gtzjmbkggi.html

echo $((1 + 2 * 3))
来源：http://hz.daxiang520.top/gtcciealnn.html

[R28] 浮点运算
来源：http://hz.gzhubu.top/gttmvyecpg.html

echo "scale=2; 10/3" | bc
来源：http://hz.yj20258.top/gtxocjyudw.html

[R29] 定义函数
来源：http://hz.ydzc1.top/gtetloifkt.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.sxryk.cn/gthofleqbi.html

[R30] 函数返回状态码
来源：http://hz.quarkkingdee.top/gtzswwqdfm.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.0kj1m.cn/gtjwaerhfj.html

[R31] 局部变量
来源：http://hz.vqdsnc.cn/gtwjlzpudz.html

f() { local x=1; echo "$x"; }
来源：http://hz.feifeiyinyue.top/gtpxoeaijx.html

[R32] 参数个数校验
来源：http://hz.hfpthk.cn/gtlivqeqvj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.gaohongyu789.top/gtbrwptkgf.html

[R33] 捕获错误并提示行号
来源：http://hz.guowangkeji.top/gtrijvpgoe.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.havefunace.top/gtcqcobsbl.html

[R34] 退出时清理
来源：http://hz.smart0.xyz/gtmurlmigf.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yvedp.cn/gtrbnfpwmo.html

[R35] 后台执行并等待
来源：http://hz.jiagoushi.top/gtqnljaxxh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.sufxvd.cn/gtibtxulfg.html

[R36] 并发执行多个任务
来源：http://hz.jlsjyb.cn/gtscjshlbg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.ydjk.org.cn/gtjquyttdl.html

[R37] 把输出赋给变量
来源：http://hz.cashguo.top/gtlzzguznu.html

files=$(ls -1)
来源：http://hz.pengpengdd.cyou/gtswgxgihq.html

[R38] 管道串联
来源：http://hz.zhaomingkeji.xyz/gtsazkctsq.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jinqigfzy.top/gtdckbptlb.html

[R39] 重定向标准输出与错误
来源：http://hz.nanxuanxn.top/gtyihpqjqo.html

cmd > out.log 2>&1
来源：http://hz.bjfxy.top/gtekiaoctw.html

[R40] 追加写日志
来源：http://hz.hnxiangtu.top/gteykofyzm.html

echo "log" >> out.log
来源：http://hz.hongshengwenyu.top/gtemkfreza.html

[R41] 丢弃输出
来源：http://hz.quarkkingdee.top/gtecpwynhb.html

cmd >/dev/null 2>&1
来源：http://hz.nwbrower.top/gtxyfotkra.html

[R42] 输入重定向
来源：http://hz.zhengqikj.top/gtnylfgbkh.html

wc -l < a.txt
来源：http://hz.ydjk.org.cn/gtprprrmux.html

[R43] 按名字查找文件
来源：http://hz.sysykeji.top/gthkywldpg.html

find . -name "*.log" -type f
来源：http://hz.tian-w.cn/gthsdodiys.html

[R44] 按修改时间查找
来源：http://hz.ydzc1.top/gteaosskel.html

find . -mtime -7 -type f
来源：http://hz.hongshengwenyu.top/gtllmpbdyj.html

[R45] 批量删除
来源：http://hz.birdmap.top/gtbsbssydz.html

find . -name "*.tmp" -delete
来源：http://hz.yvedp.cn/gtzrgiidjc.html

[R46] 递归替换文件内容
来源：http://hz.xinyue.icu/gtlytqrlaz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.cdnleiting.top/gtoiowsday.html

[R47] sed 单行替换
来源：http://hz.316326.xyz/gtyqkloyvv.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.shzxlz.cn/gturrjjyuk.html

[R48] awk 取指定列
来源：http://hz.birdmap.top/gtwzcanxbu.html

awk '{print $1, $3}' a.txt
来源：http://hz.bjfxy.top/gtpvqfmtdg.html

[R49] awk 带条件
来源：http://hz.yj202588.top/gtwzyjbelx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.xziqi.cn/gtjeoqjuiw.html

[R50] awk 求和
来源：http://hz.smart0.xyz/gtoqwlsacf.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.zhoulong.xyz/gtpcxjvrjn.html

[R51] 排序去重取前几
来源：http://hz.xinyue.icu/gtlqrqnmgl.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.fzhhl.top/gtuiuhgpgw.html

[R52] 统计行数
来源：http://hz.yuxming.cn/gtfyzpiuim.html

wc -l a.txt
来源：http://hz.xinyue.icu/gtjidwwbtb.html

[R53] 查看文件头与实时尾
来源：http://hz.xziqi.cn/gtpofzsmkh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.tian-w.cn/gtvqkfvgmv.html

[R54] 比较两个文件
来源：http://hz.havefunace.top/gtqexxwzkt.html

diff a.txt b.txt
来源：http://hz.c1oappe.top/gtpzmslyri.html

[R55] 压缩与解压
来源：http://hz.fzhhl.top/gttvyovkho.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.jqgfzy.top/gtgarnuqlw.html

[R56] 远程拷贝
来源：http://hz.ybcxt.top/gtzqyukmyk.html

scp file user@host:/path/
来源：http://hz.ehwqpu.com/gtxfkonmup.html

[R57] 远程执行命令
来源：http://hz.jinyuanbaomall.cn/gtumsulwwz.html

ssh user@host 'uptime'
来源：http://hz.yanxiufei.cn/gtnpfizhus.html

[R58] 下载文件
来源：http://hz.sweek.top/gtyuksyais.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.yanxiufei.cn/gtnceancom.html

[R59] 发 POST JSON
来源：http://hz.zhoulong.xyz/gtixjxvndo.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.xingfuxueyuan.xyz/gtmzzwdqjg.html

[R60] 只看 HTTP 状态码
来源：http://hz.nwbrower.top/gtebtidgaz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.aizwys.cn/gtpqnhiqws.html

[R61] 磁盘占用
来源：http://hz.9152youxi.cn/gtmubmfbze.html

df -h;  du -sh *
来源：http://hz.9152youxi.cn/gthymfgfuh.html

[R62] 找最占空间的文件
来源：http://hz.mhx1999.top/gtlhwbjphr.html

du -ah . | sort -rh | head -10
来源：http://hz.xylfe.cn/gthpcrztmr.html

[R63] 内存与进程
来源：http://hz.0kj1m.cn/gtlzidqvqm.html

free -h;  ps aux | grep nginx
来源：http://hz.jqgufenzy.top/gtphpmclyh.html

[R64] 结束进程
来源：http://hz.cdnleiting.top/gtwcfstufr.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jinqigfzy.top/gthurbwngn.html

[R65] 查看端口占用
来源：http://hz.zhoulong.xyz/gtxaxpdmto.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.havefunace.top/gtsoydsiuv.html

[R66] 定时任务
来源：http://hz.yueranfly.top/gtqgfvjqfs.html

crontab -e;  crontab -l
来源：http://hz.iojbl.cn/gtprdrpilw.html

[R67] 生成随机十六进制串
来源：http://hz.ehwqpu.com/gtllzbfzkn.html

openssl rand -hex 16
来源：http://hz.smart0.xyz/gtjvwlfigg.html

[R68] 计算文件校验值
来源：http://hz.zhengqikj.top/gtgipntxck.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.ydjk.org.cn/gtyvvwdole.html

[R69] 生成随机密码
来源：http://hz.pycfn.com/gtjxjwnwyq.html

head -c 16 /dev/urandom | base64
来源：http://hz.yuxming.cn/gtbauhdguu.html

[R70] 时间戳与互转
来源：http://hz.xinyue.icu/gtmycjisaq.html

date +%s;  date -d @1700000000
来源：http://hz.fengsongda.top/gtcrcfnvwc.html

[R71] 日期格式化
来源：http://hz.shzxlz.cn/gtsfscyjqh.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yuanzhike.top/gtzidqewle.html

[R72] 等待端口就绪
来源：http://hz.pycfn.com/gtlejnsojk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.cucudq.cn/gtixhohxah.html

[R73] 分割大日志
来源：http://hz.chenlongwang.top/gtxwzptugh.html

split -l 1000 big.log part_
来源：http://hz.zycfv.cn/gtjnivtzyi.html

[R74] 批量重命名
来源：http://hz.jyoumei.cn/gtgyrlzwlz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.ywan-chungtsiang.top/gtiyjhxrte.html

[R75] 导出环境变量
来源：http://hz.tianlin.xyz/gtdrtdzyjv.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.sufxvd.cn/gtpdsgizfw.html

[R76] 使用临时文件
来源：http://hz.tian-w.cn/gtbsxefzqe.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yueranfly.top/gtrgbeqsun.html

[R77] 读取用户输入
来源：http://hz.jqgufenzy.top/gtwpnwgqkq.html

read -rp "请输入: " ans
来源：http://hz.shzxlz.cn/gttattbxoo.html

[R78] 交互式菜单
来源：http://hz.iojbl.cn/gtaffgjmre.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.c1oappe.top/gtpqpprqtv.html

[R79] 解析命令行选项
来源：http://hz.havefunace.top/gtgcbcfckx.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.tian-w.cn/gthwzjqsfc.html

[R80] 查看脚本执行耗时
来源：http://hz.hongshengwenyu.top/gtshamnwoq.html

time ./run.sh
来源：http://hz.shuidangran.top/gtiypxndip.html

================================================================================
来源：http://hz.cdnleiting.top/gttcyijnbg.html

S. C / C++ 专题
来源：http://hz.tian-w.cn/gtbuxobfnu.html

================================================================================
来源：http://hz.yvedp.cn/gtdgoumdnj.html

[S01] C：Hello World
来源：http://hz.hongshengwenyu.top/gtrgxxhfmr.html

#include <stdio.h>
来源：http://hz.andypj.xyz/gtgrcaejut.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.sweek.top/gtndzlqiyn.html

[S02] C：变量与格式化输出
来源：http://hz.0kj1m.cn/gtgecfbeil.html

int a = 10; printf("%d\n", a);
来源：http://hz.nwbrower.top/gtejhbkahk.html

[S03] C：读入整数
来源：http://hz.zhaomingkeji.xyz/gtrxuqixyt.html

int x; scanf("%d", &x);
来源：http://hz.52xcode.cn/gtkxecghzj.html

[S04] C：字符串复制
来源：http://hz.haohaochexian.top/gtddehccbk.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jyoumei.cn/gtogofghvt.html

[S05] C：字符串长度
来源：http://hz.zhaomingkeji.xyz/gtqaasrfyc.html

strlen(s)
来源：http://hz.jinyuanbaomall.cn/gtdvxssewu.html

[S06] C：字符串比较
来源：http://hz.shzxlz.cn/gtktjtzqtz.html

strcmp(a, b) == 0
来源：http://hz.meibo888.top/gtapgmubat.html

[S07] C：数组遍历求和
来源：http://hz.ybcxt.top/gtmrvphvnz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.chenzaomai.com/gtzhynwyfa.html

[S08] C：动态内存分配与释放
来源：http://hz.jlsjyb.cn/gtlefgvhfg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.kuanghao11.cn/gtzrcheitc.html

[S09] C：结构体定义与初始化
来源：http://hz.hysaishi.cn/gtotqahbfu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.hammf.cn/gttpbwcaxa.html

[S10] C：指针与解引用
来源：http://hz.yvedp.cn/gthrlpqrqo.html

int *p = &a;  *p = 5;
来源：http://hz.ybcxt.top/gtcwpaflwx.html

[S11] C：逐行读文件
来源：http://hz.yj20258.top/gtrrulwjob.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jinqigfzy.top/gtyafrgkkd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.ppjwa.cn/gtsdexxzmk.html

fclose(f);
来源：http://hz.yanxiufei.cn/gtaqztswwg.html

[S12] C：写文件
来源：http://hz.sweek.top/gtsdrtnywr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.hongshengwenyu.top/gtnkuglpox.html

[S13] C：宏定义
来源：http://hz.yvedp.cn/gtcotwxlif.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.svipenyu.cn/gtbbwxnwho.html

[S14] C：枚举
来源：http://hz.hfpthk.cn/gtwhdgirbi.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yvedp.cn/gtudirviag.html

[S15] C：类型转换
来源：http://hz.hfpthk.cn/gtekuegufn.html

(double) a / b
来源：http://hz.yongpay.top/gtucslpopi.html

[S16] C：位操作置位
来源：http://hz.chenzaomai.com/gtqlhfkzim.html

x |= (1 << 3);
来源：http://hz.chenzaomai.com/gtszjxafxu.html

[S17] C：安全拼接字符串
来源：http://hz.c1oappe.top/gtzycztpit.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.nanxinkj.top/gthbbnnbwc.html

[S18] C：命令行参数
来源：http://hz.mhx1999.top/gtykfqnbdh.html

int main(int argc, char **argv)
来源：http://hz.ppjwa.cn/gtnnrtqrqp.html

[S19] C：快速排序
来源：http://hz.snrcjt.cn/gtmnbrucdc.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jlsjyb.cn/gtenfpupxb.html

[S20] C：二分查找
来源：http://hz.zhengqikj.top/gteztplabp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.shuidangran.top/gtewpofwmv.html

[S21] C：字符类别判断
来源：http://hz.zhaomingkeji.xyz/gtuebzylyk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jianghu66.top/gtytuqqnjl.html

[S22] C：字符串转数字
来源：http://hz.smart0.xyz/gtcxteybnw.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.shzxlz.cn/gttxizfxqi.html

[S23] C：随机数
来源：http://hz.zhengqikj.top/gtncufoknn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.jiagoushi.top/gthxtppzab.html

[S24] C：获取本地时间
来源：http://hz.nanxinkj.top/gtjawhucfn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.chenlongwang.top/gtigxedspq.html

[S25] C：内存拷贝
来源：http://hz.0kj1m.cn/gtdnrcvgxx.html

memcpy(dst, src, n);
来源：http://hz.nanxuanxn.top/gtsszeahff.html

[S26] C：内存清零
来源：http://hz.jinqigufen.top/gtcplxzodj.html

memset(a, 0, sizeof a);
来源：http://hz.meibo888.top/gtvbtkugkl.html

[S27] C：定义常量
来源：http://hz.gotoacloud.top/gtzxbfjswf.html

const double PI = 3.14159;
来源：http://hz.smart0.xyz/gtzkxetehh.html

[S28] C：静态变量
来源：http://hz.dianchejie.cn/gtmwjldfrn.html

static int counter = 0;
来源：http://hz.cdnleiting.top/gtawfdtdvs.html

[S29] C：变参函数
来源：http://hz.chenjidiqi.icu/gtdbzlslmm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.hnqzz.top/gtpnuwzxsh.html

[S30] C：头文件保护
来源：http://hz.tianlin.xyz/gthnuuzsbg.html

#ifndef X_H
来源：http://hz.tianlin.xyz/gtwvuqudwj.html

#define X_H
来源：http://hz.gotoacloud.top/gtwbkjwlvg.html

#endif
来源：http://hz.ydjk.org.cn/gtyfqzuvod.html

[S31] C++：Hello World
来源：http://hz.zhaomingkeji.xyz/gtyzrezsno.html

#include <iostream>
来源：http://hz.ydzc1.top/gtqttmysuu.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.jqgufenzy.top/gtrwzgygvh.html

[S32] C++：字符串
来源：http://hz.yvedp.cn/gtpjznialb.html

std::string s = "hi";  s += "!";
来源：http://hz.zhixingplan.top/gtizevjjmc.html

[S33] C++：vector 增删
来源：http://hz.yuxming.cn/gtvzzfapxb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.xuanzx.com/gtakmroiff.html

[S34] C++：遍历 vector
来源：http://hz.quarkkingdee.top/gttytkecuf.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.c1oappe.top/gtxktocglh.html

[S35] C++：map
来源：http://hz.chenzaomai.com/gtwtxpjzox.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xingfuxueyuan.xyz/gtnamrfwpr.html

[S36] C++：unordered_map
来源：http://hz.yanxiufei.cn/gtowuxtjvv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.chenzaomai.com/gtdmhdrzel.html

[S37] C++：set
来源：http://hz.cheryme.top/gtpdonovfb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.ehwqpu.com/gtuzcvwryz.html

[S38] C++：排序
来源：http://hz.hfpthk.cn/gtyupiicfa.html

std::sort(v.begin(), v.end());
来源：http://hz.mhx1999.top/gtdpsdxdif.html

[S39] C++：自定义比较器排序
来源：http://hz.hysaishi.cn/gtygnztwmx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.ydjk.org.cn/gtpsjcmsja.html

[S40] C++：查找元素
来源：http://hz.yuxming.cn/gttrgdwkzm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.tianlin.xyz/gtjuamuowl.html

[S41] C++：类与构造函数
来源：http://hz.yangfankeji.com/gtqpnuovge.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.ehwqpu.com/gtfinmvjye.html

[S42] C++：继承与虚函数
来源：http://hz.smart0.xyz/gtrkfvnsvu.html

class B : public Base { public: void f() override {} };
来源：http://hz.bjfxy.top/gtcknwzgpa.html

[S43] C++：智能指针
来源：http://hz.xuetiantiany.cn/gtylzmlftd.html

auto p = std::make_unique<int>(5);
来源：http://hz.ehwqpu.com/gtpwuuxylo.html

[S44] C++：引用传参
来源：http://hz.yongpay.top/gtprwgrxvz.html

void inc(int &x) { ++x; }
来源：http://hz.jianghu66.top/gtquqydleg.html

[S45] C++：lambda
来源：http://hz.bjfxy.top/gtbbrmtefu.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.ydjk.org.cn/gtebtdanww.html

[S46] C++：函数模板
来源：http://hz.jinqigfzy.top/gtupwqyvpw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.52xcode.cn/gtnecsfens.html

[S47] C++：结构化绑定遍历
来源：http://hz.gotoacloud.top/gtebuytaxm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.smart0.xyz/gtpcrliyyw.html

[S48] C++：逐行读文件
来源：http://hz.sysykeji.top/gtgtqalttq.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yonumen.top/gttlnawusq.html

while (std::getline(in, line)) { }
来源：http://hz.chenjidiqi.icu/gtktfqmney.html

[S49] C++：写文件
来源：http://hz.hywenlv.cn/gtbqymackg.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.shanyushiyangtech.top/gtptoqhhok.html

[S50] C++：格式化数字
来源：http://hz.jinghuilouyu.cn/gtoqdpesvj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.haohaochexian.top/gtvqgyooms.html

[S51] C++：显式类型转换
来源：http://hz.wangshuangyany.cn/gtlyypxgtw.html

static_cast<double>(a) / b
来源：http://hz.smart0.xyz/gterhrzsxa.html

[S52] C++：const 与 noexcept
来源：http://hz.shuidangran.top/gtoeestxdv.html

int size() const noexcept { return n_; }
来源：http://hz.sysykeji.top/gtnxmmneje.html

[S53] C++：移动语义
来源：http://hz.xuanzx.com/gtgdukpiob.html

std::vector<int> w = std::move(v);
来源：http://hz.cdnleiting.top/gtoysajroj.html

[S54] C++：异常处理
来源：http://hz.jyoumei.cn/gtxifaykib.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.shzxlz.cn/gtuyxzcdeu.html

[S55] C++：结构化绑定
来源：http://hz.sxryk.cn/gtupsslfrj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.jinghuilouyu.cn/gtlzoqjcco.html

[S56] C++：optional
来源：http://hz.xingfuxueyuan.xyz/gtzjcirdjd.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.pycfn.com/gtnlnlnavy.html

[S57] C++：编译期常量
来源：http://hz.aibaodan.cn/gttctufdfz.html

constexpr int N = 10;
来源：http://hz.shanyushiyangtech.top/gtumwotbbq.html

[S58] C++：命名空间
来源：http://hz.quarkkingdee.top/gtnhipjcwv.html

namespace ns { int f() { return 1; } }
来源：http://hz.shangyingyoupin.top/gtyhumanmp.html

[S59] C++：静态断言
来源：http://hz.xuanzx.com/gtiljprytu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jqgfzy.top/gtfqmplyac.html

[S60] C++：遍历并删除元素
来源：http://hz.cqqwz.cn/gthjrjjlgm.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jinyuanbaomall.cn/gtcnqgmizy.html

================================================================================
来源：http://hz.yongpay.top/gttqmzimip.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.tianlin.xyz/gtflweaqxu.html

================================================================================
来源：http://hz.pycfn.com/gtzlsixaya.html

[T01] Kotlin：Hello World
来源：http://hz.cheryme.top/gtbgyimbfd.html

println("Hello")
来源：http://hz.smart0.xyz/gtdzszjoyw.html

[T02] Kotlin：变量
来源：http://hz.xuetiantiany.cn/gtqhqsvnft.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.ydjk.org.cn/gtzhhjeotu.html

[T03] Kotlin：字符串模板
来源：http://hz.snrcjt.cn/gtilndvlij.html

"值: $b"
来源：http://hz.yangfankeji.com/gtsmhacorw.html

[T04] Kotlin：空安全
来源：http://hz.chenzaomai.com/gtfgcisuww.html

val n: String? = null;  n?.length
来源：http://hz.redwolf501.top/gtzbsichmm.html

[T05] Kotlin：when 表达式
来源：http://hz.tian-w.cn/gthndhbwyq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.c1oappe.top/gtmfemddhi.html

[T06] Kotlin：集合映射
来源：http://hz.dianchejie.cn/gtmheaozug.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.ydjk.org.cn/gtghzozrsg.html

[T07] Kotlin：集合过滤
来源：http://hz.tanke756.top/gtyjqlsevs.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.sxryk.cn/gtasswptnj.html

[T08] Kotlin：数据类
来源：http://hz.zdqjudy.top/gtnsmhawxv.html

data class User(val name: String, val age: Int)
来源：http://hz.smart0.xyz/gtmcbrzckt.html

[T09] Kotlin：扩展函数
来源：http://hz.nanxinkj.top/gtehototbz.html

fun String.exclaim() = this + "!"
来源：http://hz.meibo888.top/gtnrjrqukh.html

[T10] Kotlin：默认参数
来源：http://hz.zycfv.cn/gtxsivsneu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.tianlin.xyz/gtvmexnvnz.html


<!-- 参考信息 -->