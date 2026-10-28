代发 wailian999

name="${1:-default}"
来源：http://hz.zhiwuduotai.top/gtfjuodeaa.html

[R06] 判断命令是否存在
来源：http://hz.haohaochexian.top/gtlttdchsp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.snrcjt.cn/gtjcpymcmf.html

[R07] if 判断文件
来源：http://hz.pycfn.com/gtzzpaoojf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.mhx1999.top/gtrkjfpvde.html

[R08] 数值比较
来源：http://hz.zycfv.cn/gtqxpqarsm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.pengpengdd.cyou/gtnobhvobv.html

[R09] 字符串比较
来源：http://hz.shuidangran.top/gttlgmrcys.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zhixingplan.top/gtlgtjjwwc.html

[R10] 正则匹配
来源：http://hz.cheryme.top/gtroflztsp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jinghuilouyu.cn/gtyyflqugn.html

[R11] case 多分支
来源：http://hz.cqqwz.cn/gturnhehqm.html

case "$1" in
来源：http://hz.cheryme.top/gtcwhwaqkj.html

start) echo "启动" ;;
来源：http://hz.zhoulong.xyz/gtwaoggelc.html

stop)  echo "停止" ;;
来源：http://hz.cdnleiting.top/gtbkerspnd.html

*)     echo "未知命令" ;;
来源：http://hz.meibo888.top/gtqlifxwjn.html

esac
来源：http://hz.meibo888.top/gtunxqxusi.html

[R12] for 遍历文件
来源：http://hz.c1oappe.top/gtgfixzupe.html

for f in *.txt; do echo "$f"; done
来源：http://hz.wangshuangyany.cn/gtutuaipsc.html

[R13] for 计数循环
来源：http://hz.zhixingplan.top/gtbgdfffxo.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.aibaodan.cn/gtkivbiclt.html

[R14] C 风格 for
来源：http://hz.bjfxy.top/gtvymboems.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.smart0.xyz/gtnkgbfosh.html

[R15] while 逐行读文件
来源：http://hz.pengpengdd.cyou/gtaalkvdxg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.birdmap.top/gthhkwmwbl.html

[R16] until 等待条件
来源：http://hz.hongshengwenyu.top/gtxkdrowph.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.shangyingyoupin.top/gtnipykewr.html

[R17] 数组定义与取值
来源：http://hz.xingfuxueyuan.xyz/gtvjxkdxml.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.dianchejie.cn/gtjwijtqbw.html

[R18] 遍历数组
来源：http://hz.gogol.net.cn/gtunceuqnl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.sweek.top/gtwscepuuv.html

[R19] 数组长度
来源：http://hz.ydzc1.top/gtunheuduh.html

echo "${#arr[@]}"
来源：http://hz.pengpengdd.cyou/gtgshgecjo.html

[R20] 关联数组（字典）
来源：http://hz.zhiwuduotai.top/gtfndgzpop.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.hammf.cn/gtvhnouriw.html

[R21] 字符串长度
来源：http://hz.xziqi.cn/gtewjsxfip.html

echo "${#s}"
来源：http://hz.hysaishi.cn/gtwbylagmh.html

[R22] 截取子串
来源：http://hz.jinyuanbaomall.cn/gtmjcjksdu.html

echo "${s:0:5}"
来源：http://hz.yuanzhike.top/gtjhyzvhny.html

[R23] 字符串替换
来源：http://hz.wangshuangyany.cn/gtpoxauhju.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.xuanzx.com/gtvwycozlt.html

[R24] 大小写转换
来源：http://hz.chenlongwang.top/gtgtpxwjfi.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yongpay.top/gtumygbivh.html

[R25] 去后缀 / 去前缀
来源：http://hz.zhiwuduotai.top/gtzubnnuds.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.smart0.xyz/gtbewyrerb.html

[R26] 命令替换
来源：http://hz.shzxlz.cn/gtdnyfhixr.html

now=$(date +%F); echo "$now"
来源：http://hz.xziqi.cn/gtnazdrdrz.html

[R27] 算术展开
来源：http://hz.feifeiyinyue.top/gtcxyawvcs.html

echo $((1 + 2 * 3))
来源：http://hz.ybcxt.top/gtrbezehcr.html

[R28] 浮点运算
来源：http://hz.feifeiyinyue.top/gtpxuqxybu.html

echo "scale=2; 10/3" | bc
来源：http://hz.fzhhl.top/gtczakplhd.html

[R29] 定义函数
来源：http://hz.shanyushiyangtech.top/gtmxcqwulr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.hysaishi.cn/gtqhgyvlst.html

[R30] 函数返回状态码
来源：http://hz.shanyushiyangkeji.top/gtwyemhqga.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.zhijiandao.cn/gtpguntzeh.html

[R31] 局部变量
来源：http://hz.kuanghao11.cn/gtyrfkirec.html

f() { local x=1; echo "$x"; }
来源：http://hz.ehwqpu.com/gttrtglbmm.html

[R32] 参数个数校验
来源：http://hz.guowangkeji.top/gtnkcuczsm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.shangyingyoupin.top/gtzpzxvjcv.html

[R33] 捕获错误并提示行号
来源：http://hz.dianchejie.cn/gttnfupqrf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.nwbrower.top/gtkzendczz.html

[R34] 退出时清理
来源：http://hz.nanxinkj.top/gtkdqvxpye.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.pycfn.com/gtvfxemvvp.html

[R35] 后台执行并等待
来源：http://hz.kuanghao11.cn/gtfkmaxlkv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yanxiufei.cn/gtwojhwhiy.html

[R36] 并发执行多个任务
来源：http://hz.hnxiangtu.top/gtqzuprcmv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.sweek.top/gthxnbkcsi.html

[R37] 把输出赋给变量
来源：http://hz.ywan-chungtsiang.top/gtsszmzdug.html

files=$(ls -1)
来源：http://hz.ehwqpu.com/gtqqldxbew.html

[R38] 管道串联
来源：http://hz.zhaomingkeji.xyz/gtxbgswdrs.html

cat a.txt | grep -i error | wc -l
来源：http://hz.meibo888.top/gtonhqkfzs.html

[R39] 重定向标准输出与错误
来源：http://hz.xuetiantiany.cn/gtcnnldjgd.html

cmd > out.log 2>&1
来源：http://hz.hysaishi.cn/gthihqpwgo.html

[R40] 追加写日志
来源：http://hz.yanxiufei.cn/gtetntmzem.html

echo "log" >> out.log
来源：http://hz.zdqjudy.top/gtcajztgpi.html

[R41] 丢弃输出
来源：http://hz.chenzaomai.com/gtzhkqlyaq.html

cmd >/dev/null 2>&1
来源：http://hz.cqqwz.cn/gtumhvyoah.html

[R42] 输入重定向
来源：http://hz.yueranfly.top/gtqwyfqzyl.html

wc -l < a.txt
来源：http://hz.xuetiantiany.cn/gtkimisrmu.html

[R43] 按名字查找文件
来源：http://hz.gogol.net.cn/gtpjdevevq.html

find . -name "*.log" -type f
来源：http://hz.yvedp.cn/gthwoaqpra.html

[R44] 按修改时间查找
来源：http://hz.zhoulong.xyz/gtnmadqpbu.html

find . -mtime -7 -type f
来源：http://hz.zycfv.cn/gtzvomonkf.html

[R45] 批量删除
来源：http://hz.zhengqikj.top/gtphjlovlt.html

find . -name "*.tmp" -delete
来源：http://hz.snrcjt.cn/gtprngsnpm.html

[R46] 递归替换文件内容
来源：http://hz.yonumen.top/gtvbermjsz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.bjfxy.top/gttelxlsrp.html

[R47] sed 单行替换
来源：http://hz.zhixingplan.top/gtcigakblo.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.haohaochexian.top/gtmtioiyqq.html

[R48] awk 取指定列
来源：http://hz.yvedp.cn/gtncqbwhok.html

awk '{print $1, $3}' a.txt
来源：http://hz.cashguo.top/gtkejudida.html

[R49] awk 带条件
来源：http://hz.feifeiyinyue.top/gtieczddsl.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.xuetiantiany.cn/gtjbmumkqv.html

[R50] awk 求和
来源：http://hz.ydzc1.top/gtrysklumk.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.shanyushiyangkeji.top/gtajqhbsar.html

[R51] 排序去重取前几
来源：http://hz.aizwys.cn/gthktlenmz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jiagoushi.top/gtgpdqfpzi.html

[R52] 统计行数
来源：http://hz.bjfxy.top/gtypkjxbrg.html

wc -l a.txt
来源：http://hz.ppjwa.cn/gtafxdsuql.html

[R53] 查看文件头与实时尾
来源：http://hz.nanxinkj.top/gtiaxirfay.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.zhaomingkeji.xyz/gtzohycgsy.html

[R54] 比较两个文件
来源：http://hz.cheryme.top/gtldrupebh.html

diff a.txt b.txt
来源：http://hz.9152youxi.cn/gtganqeqho.html

[R55] 压缩与解压
来源：http://hz.yj202588.top/gtjpqsqkhf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.cqqwz.cn/gtogjlhilb.html

[R56] 远程拷贝
来源：http://hz.xziqi.cn/gtxlvkgwmb.html

scp file user@host:/path/
来源：http://hz.guannengcc.top/gtsjdzwsse.html

[R57] 远程执行命令
来源：http://hz.sweek.top/gtshmzmaao.html

ssh user@host 'uptime'
来源：http://hz.guannengcc.top/gtcvxyidso.html

[R58] 下载文件
来源：http://hz.cashguo.top/gtdhglaysp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.gzhubu.top/gtmlczicui.html

[R59] 发 POST JSON
来源：http://hz.ybcxt.top/gtmkntwlbn.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.zhengqikj.top/gtfsylpwtw.html

[R60] 只看 HTTP 状态码
来源：http://hz.zycfv.cn/gtirnmvyoq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.yonumen.top/gtjghanyaf.html

[R61] 磁盘占用
来源：http://hz.ydzc1.top/gtrzbormsk.html

df -h;  du -sh *
来源：http://hz.xziqi.cn/gtnlfikqla.html

[R62] 找最占空间的文件
来源：http://hz.ybcxt.top/gtdwiuptsy.html

du -ah . | sort -rh | head -10
来源：http://hz.yj20258.top/gtyraphywz.html

[R63] 内存与进程
来源：http://hz.sufxvd.cn/gtvkaacmhh.html

free -h;  ps aux | grep nginx
来源：http://hz.chenjidiqi.icu/gtlbykckoh.html

[R64] 结束进程
来源：http://hz.aizwys.cn/gtcsqizval.html

kill -9 $(pgrep -f app.py)
来源：http://hz.ppjwa.cn/gtuieigwrz.html

[R65] 查看端口占用
来源：http://hz.bjfxy.top/gtbxznksjz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.xingfuxueyuan.xyz/gttltximsf.html

[R66] 定时任务
来源：http://hz.zhoulong.xyz/gtzqpntalh.html

crontab -e;  crontab -l
来源：http://hz.yvedp.cn/gtfgxjuppk.html

[R67] 生成随机十六进制串
来源：http://hz.gzhubu.top/gtssxamuwf.html

openssl rand -hex 16
来源：http://hz.jinqigufen.top/gthwhbbkdh.html

[R68] 计算文件校验值
来源：http://hz.hysaishi.cn/gtghpbzbap.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.daria6918.cn/gtlycpzska.html

[R69] 生成随机密码
来源：http://hz.xuanzx.com/gtswoaxlfq.html

head -c 16 /dev/urandom | base64
来源：http://hz.haohaochexian.top/gtacuvubdq.html

[R70] 时间戳与互转
来源：http://hz.daria6918.cn/gtpbwvbipo.html

date +%s;  date -d @1700000000
来源：http://hz.vqdsnc.cn/gtxygqibcs.html

[R71] 日期格式化
来源：http://hz.aizwys.cn/gtuxdzflpj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.zhoulong.xyz/gtprjdhsgq.html

[R72] 等待端口就绪
来源：http://hz.yj20258.top/gtvyxrzbde.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.aizwys.cn/gtwcevetvi.html

[R73] 分割大日志
来源：http://hz.c1oappe.top/gtubtjlbyo.html

split -l 1000 big.log part_
来源：http://hz.guowangkeji.top/gtkbiqqhjt.html

[R74] 批量重命名
来源：http://hz.zhongyouzk.top/gtmfuizuje.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jqgufenzy.top/gtpjgphlkz.html

[R75] 导出环境变量
来源：http://hz.dianchejie.cn/gtjpkcqfqw.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.hysaishi.cn/gtnxbcladi.html

[R76] 使用临时文件
来源：http://hz.xinyue.icu/gtvyreprox.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.pycfn.com/gtgqqsnmqo.html

[R77] 读取用户输入
来源：http://hz.ehwqpu.com/gthkkxlokg.html

read -rp "请输入: " ans
来源：http://hz.yj20258888.top/gtymmyurnz.html

[R78] 交互式菜单
来源：http://hz.yj20258888.top/gtpwxvsfwc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.cheryme.top/gtsuryjyoy.html

[R79] 解析命令行选项
来源：http://hz.yj20258888.top/gtalletrfr.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.gotoacloud.top/gtlvzsazwv.html

[R80] 查看脚本执行耗时
来源：http://hz.zhengqikj.top/gtaspufrcf.html

time ./run.sh
来源：http://hz.shanyushiyangkeji.top/gtaomwayez.html

================================================================================
来源：http://hz.pycfn.com/gtzauigmny.html

S. C / C++ 专题
来源：http://hz.aibaodan.cn/gtzfnximzm.html

================================================================================
来源：http://hz.shzxlz.cn/gtrpqxzbmy.html

[S01] C：Hello World
来源：http://hz.jinqigfzy.top/gtnubeffxi.html

#include <stdio.h>
来源：http://hz.ywan-chungtsiang.top/gtrpabgayt.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.cqqwz.cn/gtvdtjrpld.html

[S02] C：变量与格式化输出
来源：http://hz.gotoacloud.top/gtfrlnxbvf.html

int a = 10; printf("%d\n", a);
来源：http://hz.hysaishi.cn/gtkgmspwky.html

[S03] C：读入整数
来源：http://hz.xuetiantiany.cn/gtpbslowto.html

int x; scanf("%d", &x);
来源：http://hz.ivvv.top/gtkcqnubpx.html

[S04] C：字符串复制
来源：http://hz.ybcxt.top/gtbnjzwyci.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.tian-w.cn/gtztqcnklf.html

[S05] C：字符串长度
来源：http://hz.hnxiangtu.top/gthoylaywg.html

strlen(s)
来源：http://hz.pycfn.com/gtkauytrfz.html

[S06] C：字符串比较
来源：http://hz.xziqi.cn/gtqgncskil.html

strcmp(a, b) == 0
来源：http://hz.yangfankeji.com/gtwguohiii.html

[S07] C：数组遍历求和
来源：http://hz.cashguo.top/gtkcxasdnb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.fengsongda.top/gtziblpjwg.html

[S08] C：动态内存分配与释放
来源：http://hz.ivvv.top/gtpiflzbse.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.zhixingplan.top/gtvuzassxh.html

[S09] C：结构体定义与初始化
来源：http://hz.hammf.cn/gtkytrnktt.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.zhaomingkeji.xyz/gtkrwoudkh.html

[S10] C：指针与解引用
来源：http://hz.hysaishi.cn/gtqohmdncn.html

int *p = &a;  *p = 5;
来源：http://hz.0kj1m.cn/gtcmpnubeo.html

[S11] C：逐行读文件
来源：http://hz.bjfxy.top/gteprhfppy.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.gzhubu.top/gtyynpzsjm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.9152youxi.cn/gtfzkllnun.html

fclose(f);
来源：http://hz.xinyue.icu/gtplilwxyi.html

[S12] C：写文件
来源：http://hz.ydjk.org.cn/gtwdjedssx.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.xuetiantiany.cn/gtupdjgljd.html

[S13] C：宏定义
来源：http://hz.shangyingyoupin.top/gtubxyczyp.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.0kj1m.cn/gtwosefraq.html

[S14] C：枚举
来源：http://hz.xylfe.cn/gtmhmwpegr.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.fengsongda.top/gtnakprvgp.html

[S15] C：类型转换
来源：http://hz.fengsongda.top/gtveesaodv.html

(double) a / b
来源：http://hz.yvedp.cn/gtderpuxzb.html

[S16] C：位操作置位
来源：http://hz.gaohongyu789.top/gteawytbyr.html

x |= (1 << 3);
来源：http://hz.yj20258888.top/gtmkkupzib.html

[S17] C：安全拼接字符串
来源：http://hz.birdmap.top/gttpjjaoyf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.yonumen.top/gtpfjmvuaz.html

[S18] C：命令行参数
来源：http://hz.quarkkingdee.top/gtxbwwpvyt.html

int main(int argc, char **argv)
来源：http://hz.tian-w.cn/gtkoscngpc.html

[S19] C：快速排序
来源：http://hz.havefunace.top/gtvallptws.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jiagoushi.top/gttnbvhodc.html

[S20] C：二分查找
来源：http://hz.jlsjyb.cn/gtacnrakxe.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.daria6918.cn/gtvkcgeugq.html

[S21] C：字符类别判断
来源：http://hz.ywan-chungtsiang.top/gtvydpyhcu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.yanxiufei.cn/gtdocgeiez.html

[S22] C：字符串转数字
来源：http://hz.ywan-chungtsiang.top/gtywcksedt.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.52xcode.cn/gtxcgplvco.html

[S23] C：随机数
来源：http://hz.guannengcc.top/gthvmsfhon.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.gzhubu.top/gtvmpdyjbv.html

[S24] C：获取本地时间
来源：http://hz.jlsjyb.cn/gtpqxfxogh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.nanxuanxn.top/gtkhbmenry.html

[S25] C：内存拷贝
来源：http://hz.chenjidiqi.icu/gtvlcuxozw.html

memcpy(dst, src, n);
来源：http://hz.mhx1999.top/gtogdnaafp.html

[S26] C：内存清零
来源：http://hz.havefunace.top/gtkkygxtpe.html

memset(a, 0, sizeof a);
来源：http://hz.feifeiyinyue.top/gtmldgqwrz.html

[S27] C：定义常量
来源：http://hz.yangfankeji.com/gtwdmeummg.html

const double PI = 3.14159;
来源：http://hz.yuanzhike.top/gtsvbwzcpr.html

[S28] C：静态变量
来源：http://hz.chenlongwang.top/gtnlpraubo.html

static int counter = 0;
来源：http://hz.mhx1999.top/gtxczkwceu.html

[S29] C：变参函数
来源：http://hz.zhaomingkeji.xyz/gtutwsiclu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.yanxiufei.cn/gtwhwynhfz.html

[S30] C：头文件保护
来源：http://hz.guowangkeji.top/gtdfdoqmsc.html

#ifndef X_H
来源：http://hz.cdnleiting.top/gthwinbxda.html

#define X_H
来源：http://hz.xziqi.cn/gtwlrfpqji.html

#endif
来源：http://hz.yangfankeji.com/gtefxaopeh.html

[S31] C++：Hello World
来源：http://hz.jinqigfzy.top/gtzgatteah.html

#include <iostream>
来源：http://hz.yj20258888.top/gtfhnueobh.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.jinyuanbaomall.cn/gtoelufqih.html

[S32] C++：字符串
来源：http://hz.shuidangran.top/gtiufptrum.html

std::string s = "hi";  s += "!";
来源：http://hz.sweek.top/gtpngrkccl.html

[S33] C++：vector 增删
来源：http://hz.tanke756.top/gtfwvftlnz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.sysykeji.top/gtschkojzp.html

[S34] C++：遍历 vector
来源：http://hz.xylfe.cn/gttmzbcddh.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.ehwqpu.com/gtxnycodad.html

[S35] C++：map
来源：http://hz.tian-w.cn/gthpmmhpcs.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.gzhubu.top/gtzhabftfa.html

[S36] C++：unordered_map
来源：http://hz.zhaomingkeji.xyz/gtedqtrvrl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhaomingkeji.xyz/gtkragniqz.html

[S37] C++：set
来源：http://hz.yangfankeji.com/gtfqbloncl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.fengsongda.top/gthkmonicq.html

[S38] C++：排序
来源：http://hz.cucudq.cn/gtjivyljcr.html

std::sort(v.begin(), v.end());
来源：http://hz.hywenlv.cn/gtrfnmwccl.html

[S39] C++：自定义比较器排序
来源：http://hz.jlsjyb.cn/gtwnebnjzs.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.shanyushiyangtech.top/gtohxpwnqr.html

[S40] C++：查找元素
来源：http://hz.xuanzx.com/gtfxkkvmey.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jinyuanbaomall.cn/gtythlgzfb.html

[S41] C++：类与构造函数
来源：http://hz.guowangkeji.top/gtwpdrstxu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.zhaomingkeji.xyz/gtyeziycuq.html

[S42] C++：继承与虚函数
来源：http://hz.sweek.top/gtbbkejlzy.html

class B : public Base { public: void f() override {} };
来源：http://hz.gotoacloud.top/gtlojtkbxp.html

[S43] C++：智能指针
来源：http://hz.chenjidiqi.icu/gtpfetbvzo.html

auto p = std::make_unique<int>(5);
来源：http://hz.yvedp.cn/gtpigkgwlj.html

[S44] C++：引用传参
来源：http://hz.gaohongyu789.top/gthshpybuq.html

void inc(int &x) { ++x; }
来源：http://hz.jqgufenzy.top/gtpyrvmcre.html

[S45] C++：lambda
来源：http://hz.jlsjyb.cn/gtfkztqwff.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jqgufenzy.top/gtxpgsmkim.html

[S46] C++：函数模板
来源：http://hz.yonumen.top/gtdrwrxaiu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.fengsongda.top/gtiafkyrbx.html

[S47] C++：结构化绑定遍历
来源：http://hz.xuetiantiany.cn/gtxzpskawi.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.yvedp.cn/gtogfetfou.html

[S48] C++：逐行读文件
来源：http://hz.jiagoushi.top/gtmecxblvh.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jianghu66.top/gtdlpzqyyx.html

while (std::getline(in, line)) { }
来源：http://hz.cheryme.top/gtxbrhfdmj.html

[S49] C++：写文件
来源：http://hz.0kj1m.cn/gtuofvlqfw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.dashuyun.cn/gtgqzjsxtj.html

[S50] C++：格式化数字
来源：http://hz.yuxming.cn/gtwsgfcrvz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.vqdsnc.cn/gtpcewvhnh.html

[S51] C++：显式类型转换
来源：http://hz.ehwqpu.com/gtowubofol.html

static_cast<double>(a) / b
来源：http://hz.svipenyu.cn/gtxlrkzrcd.html

[S52] C++：const 与 noexcept
来源：http://hz.xuetiantiany.cn/gtcykufzwv.html

int size() const noexcept { return n_; }
来源：http://hz.c1oappe.top/gtcfeorqjy.html

[S53] C++：移动语义
来源：http://hz.quarkkingdee.top/gtxwjqstwo.html

std::vector<int> w = std::move(v);
来源：http://hz.hammf.cn/gteazxxgzl.html

[S54] C++：异常处理
来源：http://hz.gotoacloud.top/gtelzlyrtc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.mhx1999.top/gtpnospcuf.html

[S55] C++：结构化绑定
来源：http://hz.jinqigfzy.top/gtqjqycjfg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.shuidangran.top/gttaxxowvx.html

[S56] C++：optional
来源：http://hz.cqqwz.cn/gttynnegvj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.gaohongyu789.top/gtkgzqgzrt.html

[S57] C++：编译期常量
来源：http://hz.cashguo.top/gtsgyfrryd.html

constexpr int N = 10;
来源：http://hz.tanke756.top/gtbxsbcwem.html

[S58] C++：命名空间
来源：http://hz.ydzc1.top/gttlogqyki.html

namespace ns { int f() { return 1; } }
来源：http://hz.kuanghao11.cn/gtwhkwsrvn.html

[S59] C++：静态断言
来源：http://hz.jqgufenzy.top/gtrmqpitng.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jinyuanbaomall.cn/gtthfhgkra.html

[S60] C++：遍历并删除元素
来源：http://hz.hnqzz.top/gtcenkhocs.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.gogol.net.cn/gtigapqgcu.html

================================================================================
来源：http://hz.yueranfly.top/gtlqlcozms.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.0kj1m.cn/gtzevwszxx.html

================================================================================
来源：http://hz.daria6918.cn/gtosaoxlrq.html

[T01] Kotlin：Hello World
来源：http://hz.yangfankeji.com/gttzvofaad.html

println("Hello")
来源：http://hz.ybcxt.top/gtiwogxyxf.html

[T02] Kotlin：变量
来源：http://hz.zycfv.cn/gthpntkrfg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.chenzaomai.com/gtlgeewvru.html

[T03] Kotlin：字符串模板
来源：http://hz.ivvv.top/gtqvvyrqfh.html

"值: $b"
来源：http://hz.c1oappe.top/gtfflbhppo.html

[T04] Kotlin：空安全
来源：http://hz.hnxiangtu.top/gtefvfxdmz.html

val n: String? = null;  n?.length
来源：http://hz.ehwqpu.com/gturqqkdci.html

[T05] Kotlin：when 表达式
来源：http://hz.cashguo.top/gthdwuochq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.havefunace.top/gtadlpwywq.html

[T06] Kotlin：集合映射
来源：http://hz.zhongyouzk.top/gthznaobnp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.zhixingplan.top/gtipcpkhnh.html


<!-- 参考信息 -->