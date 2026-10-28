代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.shanyushiyangkeji.top/gtmycpoafy.html

[R08] 数值比较
来源：http://hz.jinqigfzy.top/gtlxdfbthx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.shangyingyoupin.top/gtufvcuejk.html

[R09] 字符串比较
来源：http://hz.pengpengdd.cyou/gtitwjodjx.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.9152youxi.cn/gtwwbrvcjh.html

[R10] 正则匹配
来源：http://hz.aibaodan.cn/gthyolwsbk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.ehwqpu.com/gtichsodob.html

[R11] case 多分支
来源：http://hz.dianchejie.cn/gtffqsuohq.html

case "$1" in
来源：http://hz.yuanzhike.top/gtlmgmagcx.html

start) echo "启动" ;;
来源：http://hz.tianlin.xyz/gtiggnlpxj.html

stop)  echo "停止" ;;
来源：http://hz.meibo888.top/gtmtlpsnqp.html

*)     echo "未知命令" ;;
来源：http://hz.shanyushiyangkeji.top/gtlvpkkfwd.html

esac
来源：http://hz.jinghuilouyu.cn/gtxeqlqjcx.html

[R12] for 遍历文件
来源：http://hz.zhengqikj.top/gtkhhxoklt.html

for f in *.txt; do echo "$f"; done
来源：http://hz.kuanghao11.cn/gthhnajpbc.html

[R13] for 计数循环
来源：http://hz.zhaomingkeji.xyz/gtsnbcareh.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.cucudq.cn/gttycetmyo.html

[R14] C 风格 for
来源：http://hz.shanyushiyangtech.top/gtbvupvtoq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.tianlin.xyz/gtugjfyogl.html

[R15] while 逐行读文件
来源：http://hz.c1oappe.top/gtvxggveji.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.tanke756.top/gtvkznmmbs.html

[R16] until 等待条件
来源：http://hz.sxryk.cn/gttgafjoxf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.kuanghao11.cn/gtchtpkozc.html

[R17] 数组定义与取值
来源：http://hz.hywenlv.cn/gtnmvauyzm.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.wangdashe.top/gttnssdnyo.html

[R18] 遍历数组
来源：http://hz.cashguo.top/gtvvlnfbpw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.shzxlz.cn/gtaeiqvifv.html

[R19] 数组长度
来源：http://hz.zhengqikj.top/gtpzjjelsi.html

echo "${#arr[@]}"
来源：http://hz.yj202588.top/gtlgavimte.html

[R20] 关联数组（字典）
来源：http://hz.hywenlv.cn/gtbjqwkbop.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.guannengcc.top/gtggjdgcvs.html

[R21] 字符串长度
来源：http://hz.hnqzz.top/gtwpixfxmv.html

echo "${#s}"
来源：http://hz.chenlongwang.top/gtyhgqrjqi.html

[R22] 截取子串
来源：http://hz.dianchejie.cn/gtizickayt.html

echo "${s:0:5}"
来源：http://hz.316326.xyz/gtpnavgilr.html

[R23] 字符串替换
来源：http://hz.shzxlz.cn/gtnrzjhxrn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jqgfzy.top/gtptyptqks.html

[R24] 大小写转换
来源：http://hz.xuetiantiany.cn/gtzypybulo.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.jinqigfzy.top/gtoqgwrkhg.html

[R25] 去后缀 / 去前缀
来源：http://hz.zhoulong.xyz/gtjqzordwy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.dianchejie.cn/gtiptccick.html

[R26] 命令替换
来源：http://hz.cheryme.top/gtenurkgpn.html

now=$(date +%F); echo "$now"
来源：http://hz.havefunace.top/gtewkeymgn.html

[R27] 算术展开
来源：http://hz.wangdashe.top/gtyzzoroon.html

echo $((1 + 2 * 3))
来源：http://hz.sxryk.cn/gtjzfskhti.html

[R28] 浮点运算
来源：http://hz.quarkkingdee.top/gtmwxgbscf.html

echo "scale=2; 10/3" | bc
来源：http://hz.wangshuangyany.cn/gtszofqvhf.html

[R29] 定义函数
来源：http://hz.dianchejie.cn/gtvtfwntap.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yj202588.top/gtpbjdlrwq.html

[R30] 函数返回状态码
来源：http://hz.jianghu66.top/gtkpyfavdv.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.nanxinkj.top/gtruaanenw.html

[R31] 局部变量
来源：http://hz.sysykeji.top/gtrnrhnqpd.html

f() { local x=1; echo "$x"; }
来源：http://hz.yonumen.top/gtnqpbsgst.html

[R32] 参数个数校验
来源：http://hz.jianghu66.top/gtsumsqwqu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.gaohongyu789.top/gtcjsebwei.html

[R33] 捕获错误并提示行号
来源：http://hz.zhiwuduotai.top/gtryjiffak.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.shanyushiyangkeji.top/gtxdcpnkfc.html

[R34] 退出时清理
来源：http://hz.hongshengwenyu.top/gtdbzcyxvz.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.snrcjt.cn/gtlipuiqtw.html

[R35] 后台执行并等待
来源：http://hz.chenzaomai.com/gterppsfzj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.redwolf501.top/gtbmgkqzqw.html

[R36] 并发执行多个任务
来源：http://hz.gogol.net.cn/gtrzwdxdke.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.cheryme.top/gtuefaufip.html

[R37] 把输出赋给变量
来源：http://hz.xinyue.icu/gtjcgdfxrv.html

files=$(ls -1)
来源：http://hz.feifeiyinyue.top/gtvqyapgrk.html

[R38] 管道串联
来源：http://hz.dashuyun.cn/gtgydmzhor.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yj20258888.top/gtdxdngyex.html

[R39] 重定向标准输出与错误
来源：http://hz.tian-w.cn/gtrntnqhni.html

cmd > out.log 2>&1
来源：http://hz.shzxlz.cn/gtjrszemgv.html

[R40] 追加写日志
来源：http://hz.smart0.xyz/gtpjxbkxvf.html

echo "log" >> out.log
来源：http://hz.meibo888.top/gtdrznsvqh.html

[R41] 丢弃输出
来源：http://hz.zhiwuduotai.top/gtxjymmaaq.html

cmd >/dev/null 2>&1
来源：http://hz.nanxinkj.top/gtczyswrlu.html

[R42] 输入重定向
来源：http://hz.guowangkeji.top/gtrtwtbtoe.html

wc -l < a.txt
来源：http://hz.hammf.cn/gtiumljjda.html

[R43] 按名字查找文件
来源：http://hz.zdqjudy.top/gtrpophrso.html

find . -name "*.log" -type f
来源：http://hz.zhiwuduotai.top/gthzhazjcq.html

[R44] 按修改时间查找
来源：http://hz.hnxiangtu.top/gtpouzknau.html

find . -mtime -7 -type f
来源：http://hz.yj202588.top/gtnsrwchsm.html

[R45] 批量删除
来源：http://hz.quarkkingdee.top/gtyyqapceo.html

find . -name "*.tmp" -delete
来源：http://hz.52xcode.cn/gtkycumbuk.html

[R46] 递归替换文件内容
来源：http://hz.aibaodan.cn/gtbvbuhdtn.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jinqigfzy.top/gtqknellma.html

[R47] sed 单行替换
来源：http://hz.zhoulong.xyz/gtutygelzf.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.zhengqikj.top/gtkupepluu.html

[R48] awk 取指定列
来源：http://hz.tian-w.cn/gtihpylpcz.html

awk '{print $1, $3}' a.txt
来源：http://hz.cashguo.top/gtwlpfxpoc.html

[R49] awk 带条件
来源：http://hz.ydzc1.top/gtjrayqvkw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.sxryk.cn/gtvkvkbter.html

[R50] awk 求和
来源：http://hz.shanyushiyangkeji.top/gthfimlqhg.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.jiagoushi.top/gtbcshykrf.html

[R51] 排序去重取前几
来源：http://hz.shuidangran.top/gthunoyxwk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.xziqi.cn/gtqmpcvcbx.html

[R52] 统计行数
来源：http://hz.zhaomingkeji.xyz/gtporbysbn.html

wc -l a.txt
来源：http://hz.52xcode.cn/gtbsodhvjd.html

[R53] 查看文件头与实时尾
来源：http://hz.zhixingplan.top/gtmfjzmvsm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.jinyuanbaomall.cn/gturikojva.html

[R54] 比较两个文件
来源：http://hz.zhoulong.xyz/gtacgfzuzu.html

diff a.txt b.txt
来源：http://hz.pengpengdd.cyou/gtastskhqp.html

[R55] 压缩与解压
来源：http://hz.chenzaomai.com/gtsgkmssol.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.ivvv.top/gtiwossrbt.html

[R56] 远程拷贝
来源：http://hz.gotoacloud.top/gtbflskfbd.html

scp file user@host:/path/
来源：http://hz.ydjk.org.cn/gtzigblonu.html

[R57] 远程执行命令
来源：http://hz.jinqigfzy.top/gtppsznsnn.html

ssh user@host 'uptime'
来源：http://hz.tian-w.cn/gtpfjbhaue.html

[R58] 下载文件
来源：http://hz.yangfankeji.com/gtmerzhqdx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.aizwys.cn/gtjydwnykr.html

[R59] 发 POST JSON
来源：http://hz.zhoulong.xyz/gtsoihhfze.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jlsjyb.cn/gtmconwqcw.html

[R60] 只看 HTTP 状态码
来源：http://hz.yvedp.cn/gtfaueuwrd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.wangdashe.top/gtlenzyrrw.html

[R61] 磁盘占用
来源：http://hz.0kj1m.cn/gtjjldgxsy.html

df -h;  du -sh *
来源：http://hz.redwolf501.top/gtpvosnlop.html

[R62] 找最占空间的文件
来源：http://hz.tanke756.top/gtpqjjpcon.html

du -ah . | sort -rh | head -10
来源：http://hz.yueranfly.top/gtejeozsly.html

[R63] 内存与进程
来源：http://hz.gaohongyu789.top/gtxyjmtvtk.html

free -h;  ps aux | grep nginx
来源：http://hz.nanxinkj.top/gtcohmqxok.html

[R64] 结束进程
来源：http://hz.guannengcc.top/gtftqxidnm.html

kill -9 $(pgrep -f app.py)
来源：http://hz.zhaomingkeji.xyz/gtgrrywnbr.html

[R65] 查看端口占用
来源：http://hz.daria6918.cn/gtkthvipzm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.zhengqikj.top/gtdhlbauyf.html

[R66] 定时任务
来源：http://hz.yuanzhike.top/gtjdyxqock.html

crontab -e;  crontab -l
来源：http://hz.nanxinkj.top/gtfwwyrwki.html

[R67] 生成随机十六进制串
来源：http://hz.jianghu66.top/gtgpzuxdjr.html

openssl rand -hex 16
来源：http://hz.daria6918.cn/gtpfbafsbz.html

[R68] 计算文件校验值
来源：http://hz.wangdashe.top/gtbmsrkuzy.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.feifeiyinyue.top/gtcgttuhwv.html

[R69] 生成随机密码
来源：http://hz.smart0.xyz/gttgvacdes.html

head -c 16 /dev/urandom | base64
来源：http://hz.fzhhl.top/gtcvuwnxfv.html

[R70] 时间戳与互转
来源：http://hz.havefunace.top/gtapxiibrf.html

date +%s;  date -d @1700000000
来源：http://hz.ppjwa.cn/gtjfbkoeza.html

[R71] 日期格式化
来源：http://hz.ybcxt.top/gtdgrndtfw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.feifeiyinyue.top/gttbyhdvih.html

[R72] 等待端口就绪
来源：http://hz.smart0.xyz/gtemvuyrct.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.sufxvd.cn/gtewcxsakg.html

[R73] 分割大日志
来源：http://hz.yongpay.top/gttsjbudcx.html

split -l 1000 big.log part_
来源：http://hz.cdnleiting.top/gtuozedgfc.html

[R74] 批量重命名
来源：http://hz.yanxiufei.cn/gttwjtybtc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.zhiwuduotai.top/gtdkdcfxvq.html

[R75] 导出环境变量
来源：http://hz.0kj1m.cn/gtpzidhalb.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yj20258.top/gtnptwhasv.html

[R76] 使用临时文件
来源：http://hz.hfpthk.cn/gtbdhrigol.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yueranfly.top/gtmexuhyke.html

[R77] 读取用户输入
来源：http://hz.xylfe.cn/gtywdrrlzi.html

read -rp "请输入: " ans
来源：http://hz.gotoacloud.top/gtznezxbpr.html

[R78] 交互式菜单
来源：http://hz.hfpthk.cn/gtzihvhzfk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.ydjk.org.cn/gtiuvporpx.html

[R79] 解析命令行选项
来源：http://hz.jlsjyb.cn/gtovzdecaw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.xingfuxueyuan.xyz/gtykigmbxk.html

[R80] 查看脚本执行耗时
来源：http://hz.ybcxt.top/gtddluzhpc.html

time ./run.sh
来源：http://hz.c1oappe.top/gtehhhdoxm.html

================================================================================
来源：http://hz.0kj1m.cn/gtfwwuicyr.html

S. C / C++ 专题
来源：http://hz.dianchejie.cn/gtfylzezfr.html

================================================================================
来源：http://hz.xinyue.icu/gtjpwlzten.html

[S01] C：Hello World
来源：http://hz.xuanzx.com/gtphigncsd.html

#include <stdio.h>
来源：http://hz.yuanzhike.top/gtioewzsng.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.zhiwuduotai.top/gtyapbvqsq.html

[S02] C：变量与格式化输出
来源：http://hz.pengpengdd.cyou/gtrgcqnigp.html

int a = 10; printf("%d\n", a);
来源：http://hz.jqgufenzy.top/gtegghxomo.html

[S03] C：读入整数
来源：http://hz.ydzc1.top/gtccravdxc.html

int x; scanf("%d", &x);
来源：http://hz.xinyue.icu/gtqmvemsbo.html

[S04] C：字符串复制
来源：http://hz.vqdsnc.cn/gtidoinhea.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.haohaochexian.top/gtdccbctwj.html

[S05] C：字符串长度
来源：http://hz.wangshuangyany.cn/gtitlgolzk.html

strlen(s)
来源：http://hz.haohaochexian.top/gterwknvfe.html

[S06] C：字符串比较
来源：http://hz.gzhubu.top/gtqnbcctdy.html

strcmp(a, b) == 0
来源：http://hz.9152youxi.cn/gteykfmksj.html

[S07] C：数组遍历求和
来源：http://hz.hnxiangtu.top/gtzegacwqo.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.shzxlz.cn/gtvhciyxud.html

[S08] C：动态内存分配与释放
来源：http://hz.kuanghao11.cn/gtgfnllvbo.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.ywan-chungtsiang.top/gtufmkeape.html

[S09] C：结构体定义与初始化
来源：http://hz.tian-w.cn/gtwwykfpgp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.jqgfzy.top/gtrjrhckzl.html

[S10] C：指针与解引用
来源：http://hz.hysaishi.cn/gtbemuptic.html

int *p = &a;  *p = 5;
来源：http://hz.tanke756.top/gtrsrlbful.html

[S11] C：逐行读文件
来源：http://hz.zhoulong.xyz/gtsojrvyba.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.pengpengdd.cyou/gtlzeduqgc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jinqigfzy.top/gtebdabzmw.html

fclose(f);
来源：http://hz.0kj1m.cn/gtocsimnaw.html

[S12] C：写文件
来源：http://hz.mhx1999.top/gthplpkesx.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.sysykeji.top/gtenlpsocx.html

[S13] C：宏定义
来源：http://hz.yvedp.cn/gtlxrnkzuy.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.feifeiyinyue.top/gtrrcxcqqv.html

[S14] C：枚举
来源：http://hz.jianghu66.top/gtiufjtjoz.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.ivvv.top/gtxukzpylk.html

[S15] C：类型转换
来源：http://hz.316326.xyz/gtlluhiqat.html

(double) a / b
来源：http://hz.sweek.top/gtnykvlhjl.html

[S16] C：位操作置位
来源：http://hz.shzxlz.cn/gtwazvvdey.html

x |= (1 << 3);
来源：http://hz.zhixingplan.top/gtyvbccbpp.html

[S17] C：安全拼接字符串
来源：http://hz.pycfn.com/gtqmektbpb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jlsjyb.cn/gtcdqdwtkm.html

[S18] C：命令行参数
来源：http://hz.dashuyun.cn/gtuwbmvnne.html

int main(int argc, char **argv)
来源：http://hz.yuxming.cn/gtgixfeitk.html

[S19] C：快速排序
来源：http://hz.gaohongyu789.top/gtpguzknyt.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.quarkkingdee.top/gthsaapoih.html

[S20] C：二分查找
来源：http://hz.nanxuanxn.top/gticmrjvpy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.wangdashe.top/gtfduphdcy.html

[S21] C：字符类别判断
来源：http://hz.zhixingplan.top/gtqomzcxgh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.sweek.top/gtvdgfffrz.html

[S22] C：字符串转数字
来源：http://hz.xziqi.cn/gtdbdzgguu.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.c1oappe.top/gtcvvewjcm.html

[S23] C：随机数
来源：http://hz.zhaomingkeji.xyz/gtlbnrxgvs.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.shanyushiyangkeji.top/gttnnsojer.html

[S24] C：获取本地时间
来源：http://hz.tanke756.top/gtlcdfpxze.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.bjfxy.top/gtgnidgfce.html

[S25] C：内存拷贝
来源：http://hz.vqdsnc.cn/gtvkdngiyp.html

memcpy(dst, src, n);
来源：http://hz.dashuyun.cn/gtkcaqilrn.html

[S26] C：内存清零
来源：http://hz.smart0.xyz/gtzmidstit.html

memset(a, 0, sizeof a);
来源：http://hz.jianghu66.top/gtkpvozfea.html

[S27] C：定义常量
来源：http://hz.daxiang520.top/gtkqmjahei.html

const double PI = 3.14159;
来源：http://hz.zycfv.cn/gtpxhmbsdj.html

[S28] C：静态变量
来源：http://hz.tanke756.top/gtdpiyswdi.html

static int counter = 0;
来源：http://hz.c1oappe.top/gtaycxhshe.html

[S29] C：变参函数
来源：http://hz.yongpay.top/gtzhzghczv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.yuanzhike.top/gtqiepsqct.html

[S30] C：头文件保护
来源：http://hz.dianchejie.cn/gtcxxsscck.html

#ifndef X_H
来源：http://hz.havefunace.top/gtfqrhtamq.html

#define X_H
来源：http://hz.nwbrower.top/gtcoqbujhv.html

#endif
来源：http://hz.xinyue.icu/gtsjaqxvqh.html

[S31] C++：Hello World
来源：http://hz.ydjk.org.cn/gtazdyjazh.html

#include <iostream>
来源：http://hz.smart0.xyz/gtxvgodjlw.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.andypj.xyz/gttcongses.html

[S32] C++：字符串
来源：http://hz.ehwqpu.com/gtmeqjnnkd.html

std::string s = "hi";  s += "!";
来源：http://hz.hnqzz.top/gtnltbdmvd.html

[S33] C++：vector 增删
来源：http://hz.ehwqpu.com/gtqdpfyhxc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.nanxuanxn.top/gtubydkvcz.html

[S34] C++：遍历 vector
来源：http://hz.shuidangran.top/gtheihjhkm.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.daxiang520.top/gtaxywfkse.html

[S35] C++：map
来源：http://hz.kuanghao11.cn/gtizcapeln.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yuxming.cn/gtlrenhcwd.html

[S36] C++：unordered_map
来源：http://hz.ybcxt.top/gtwpzwzqup.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.svipenyu.cn/gteyqhukpd.html

[S37] C++：set
来源：http://hz.jinghuilouyu.cn/gtigoieyoz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yangfankeji.com/gtugpzoweo.html

[S38] C++：排序
来源：http://hz.zhijiandao.cn/gtriysmlis.html

std::sort(v.begin(), v.end());
来源：http://hz.xziqi.cn/gthbawmbsw.html

[S39] C++：自定义比较器排序
来源：http://hz.hfpthk.cn/gttrlspesv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.jyoumei.cn/gtnljygssm.html

[S40] C++：查找元素
来源：http://hz.feifeiyinyue.top/gtotbdlldj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.hywenlv.cn/gtcjvrcayy.html

[S41] C++：类与构造函数
来源：http://hz.gzhubu.top/gtsjrmfnet.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.zhoulong.xyz/gtqhvlmgvj.html

[S42] C++：继承与虚函数
来源：http://hz.c1oappe.top/gtunbjcsfk.html

class B : public Base { public: void f() override {} };
来源：http://hz.yanxiufei.cn/gtzxwkhkdj.html

[S43] C++：智能指针
来源：http://hz.gotoacloud.top/gtvvpkaqzq.html

auto p = std::make_unique<int>(5);
来源：http://hz.zhengqikj.top/gtyvssjbru.html

[S44] C++：引用传参
来源：http://hz.havefunace.top/gtswthpkuu.html

void inc(int &x) { ++x; }
来源：http://hz.nanxinkj.top/gtkyyqzipu.html

[S45] C++：lambda
来源：http://hz.wangshuangyany.cn/gtzkvdwefp.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.gogol.net.cn/gtvcupasis.html

[S46] C++：函数模板
来源：http://hz.sufxvd.cn/gtxndqbexa.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zhoulong.xyz/gtqmnrwayb.html

[S47] C++：结构化绑定遍历
来源：http://hz.ydjk.org.cn/gtqebyenms.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.mhx1999.top/gtemhavdip.html

[S48] C++：逐行读文件
来源：http://hz.daria6918.cn/gtgmfkgxsy.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yj20258.top/gtaplkfwmv.html

while (std::getline(in, line)) { }
来源：http://hz.iojbl.cn/gtykyxqhcm.html

[S49] C++：写文件
来源：http://hz.aibaodan.cn/gtcsufbokt.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.zhengqikj.top/gtclhabfkt.html

[S50] C++：格式化数字
来源：http://hz.bjfxy.top/gtavvurbjw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.zhaomingkeji.xyz/gtoelvpugf.html

[S51] C++：显式类型转换
来源：http://hz.aizwys.cn/gtrqmmlgea.html

static_cast<double>(a) / b
来源：http://hz.aibaodan.cn/gtgqhhsdyg.html

[S52] C++：const 与 noexcept
来源：http://hz.zhaomingkeji.xyz/gtubtljdip.html

int size() const noexcept { return n_; }
来源：http://hz.jiagoushi.top/gttumvhlxg.html

[S53] C++：移动语义
来源：http://hz.jlsjyb.cn/gtbymuufil.html

std::vector<int> w = std::move(v);
来源：http://hz.sysykeji.top/gtomzetclx.html

[S54] C++：异常处理
来源：http://hz.hfpthk.cn/gtkwwjfcog.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.hysaishi.cn/gtrfbzebpt.html

[S55] C++：结构化绑定
来源：http://hz.cqqwz.cn/gtlckgponp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.sufxvd.cn/gtmgrvbeud.html

[S56] C++：optional
来源：http://hz.ywan-chungtsiang.top/gtmwaotgub.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.zhiwuduotai.top/gtjgqotasx.html

[S57] C++：编译期常量
来源：http://hz.nanxinkj.top/gtdylrzvtr.html

constexpr int N = 10;
来源：http://hz.cheryme.top/gtterotluh.html

[S58] C++：命名空间
来源：http://hz.cqqwz.cn/gtxiejkanz.html

namespace ns { int f() { return 1; } }
来源：http://hz.zhiwuduotai.top/gtlbtaovpg.html

[S59] C++：静态断言
来源：http://hz.zhijiandao.cn/gtmkwuqgnb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.mhx1999.top/gtoxnldgyq.html

[S60] C++：遍历并删除元素
来源：http://hz.shanyushiyangtech.top/gtlsmfifef.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.ywan-chungtsiang.top/gtagngjwct.html

================================================================================
来源：http://hz.cdnleiting.top/gtybwkzbsp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.mhx1999.top/gtfvfxsbxh.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtxplasqxn.html

[T01] Kotlin：Hello World
来源：http://hz.dianchejie.cn/gtvfgcbsdy.html

println("Hello")
来源：http://hz.316326.xyz/gttxnlsfwf.html

[T02] Kotlin：变量
来源：http://hz.yongpay.top/gttzmvryhi.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.zhongyouzk.top/gttuehdked.html

[T03] Kotlin：字符串模板
来源：http://hz.zdqjudy.top/gtberdzmnq.html

"值: $b"
来源：http://hz.cucudq.cn/gtctgbivig.html

[T04] Kotlin：空安全
来源：http://hz.ivvv.top/gtiuwqtkwt.html

val n: String? = null;  n?.length
来源：http://hz.ppjwa.cn/gtcaywpxmc.html

[T05] Kotlin：when 表达式
来源：http://hz.gzhubu.top/gtwslkbagx.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.cheryme.top/gtmbwuahfg.html

[T06] Kotlin：集合映射
来源：http://hz.dianchejie.cn/gtqurqczky.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.andypj.xyz/gtffyrylpq.html

[T07] Kotlin：集合过滤
来源：http://hz.jinyuanbaomall.cn/gtmwgyhnmq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.feifeiyinyue.top/gtsninzrjn.html

[T08] Kotlin：数据类
来源：http://hz.guannengcc.top/gtykiujbtt.html

data class User(val name: String, val age: Int)
来源：http://hz.yonumen.top/gtnissijbt.html


<!-- 参考信息 -->