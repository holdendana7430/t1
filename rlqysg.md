代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.ydjk.org.cn/gtrxfmxexf.html

[R10] 正则匹配
来源：http://hz.jyoumei.cn/gtsopwsnps.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.vqdsnc.cn/gtfrvlfbsm.html

[R11] case 多分支
来源：http://hz.hywenlv.cn/gtovdbuulf.html

case "$1" in
来源：http://hz.ydzc1.top/gtnhlkmxeb.html

start) echo "启动" ;;
来源：http://hz.fengsongda.top/gtljwqlqgn.html

stop)  echo "停止" ;;
来源：http://hz.yj202588.top/gtvumjjhjv.html

*)     echo "未知命令" ;;
来源：http://hz.bjfxy.top/gtwvisggsi.html

esac
来源：http://hz.yueranfly.top/gtziykfdbb.html

[R12] for 遍历文件
来源：http://hz.daria6918.cn/gtnmhjxwao.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yueranfly.top/gtwftgybmm.html

[R13] for 计数循环
来源：http://hz.haohaochexian.top/gtkenqzgha.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jinyuanbaomall.cn/gtfsmencjf.html

[R14] C 风格 for
来源：http://hz.pycfn.com/gtfnedjjvd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.birdmap.top/gtouwfxoiz.html

[R15] while 逐行读文件
来源：http://hz.sufxvd.cn/gtkccdwbdt.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.xuanzx.com/gtwoekpgij.html

[R16] until 等待条件
来源：http://hz.pengpengdd.cyou/gtspdzsnmn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jiagoushi.top/gtgzbdpqcf.html

[R17] 数组定义与取值
来源：http://hz.jinqigufen.top/gtltyrievl.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.daria6918.cn/gtbyvzerwe.html

[R18] 遍历数组
来源：http://hz.hysaishi.cn/gtntgianrz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.andypj.xyz/gtsihgtlim.html

[R19] 数组长度
来源：http://hz.guowangkeji.top/gtaurubwih.html

echo "${#arr[@]}"
来源：http://hz.ppjwa.cn/gtpdsvoqnv.html

[R20] 关联数组（字典）
来源：http://hz.redwolf501.top/gtebehzbqk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.shanyushiyangkeji.top/gtytffmrym.html

[R21] 字符串长度
来源：http://hz.0kj1m.cn/gtispyufsy.html

echo "${#s}"
来源：http://hz.sufxvd.cn/gtuyjlewxe.html

[R22] 截取子串
来源：http://hz.ivvv.top/gtlwgpgyse.html

echo "${s:0:5}"
来源：http://hz.pycfn.com/gttmptqjtp.html

[R23] 字符串替换
来源：http://hz.vqdsnc.cn/gterjgaeli.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.nwbrower.top/gthjxmhfok.html

[R24] 大小写转换
来源：http://hz.yanxiufei.cn/gtndfldwlj.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.xinyue.icu/gtgkwjcwzt.html

[R25] 去后缀 / 去前缀
来源：http://hz.yj202588.top/gtqlvgujsa.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.sysykeji.top/gttrmocdjd.html

[R26] 命令替换
来源：http://hz.fengsongda.top/gtjukjgaap.html

now=$(date +%F); echo "$now"
来源：http://hz.0kj1m.cn/gtqrhvydzz.html

[R27] 算术展开
来源：http://hz.yangfankeji.com/gtyctourfz.html

echo $((1 + 2 * 3))
来源：http://hz.zhongyouzk.top/gtjjjnycpy.html

[R28] 浮点运算
来源：http://hz.shanyushiyangkeji.top/gtaitfkokq.html

echo "scale=2; 10/3" | bc
来源：http://hz.c1oappe.top/gtqpouypaa.html

[R29] 定义函数
来源：http://hz.yj20258.top/gthdmluoeo.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.sysykeji.top/gtznizerns.html

[R30] 函数返回状态码
来源：http://hz.yj202588.top/gtjhjfylvo.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.daria6918.cn/gtklmniyhn.html

[R31] 局部变量
来源：http://hz.xinyue.icu/gtpcthtqfk.html

f() { local x=1; echo "$x"; }
来源：http://hz.hongshengwenyu.top/gtiyerybdi.html

[R32] 参数个数校验
来源：http://hz.gotoacloud.top/gtyucgiwnc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jlsjyb.cn/gtlkesxyjv.html

[R33] 捕获错误并提示行号
来源：http://hz.yuxming.cn/gttzfkwuxz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zhaomingkeji.xyz/gtfudsmnlo.html

[R34] 退出时清理
来源：http://hz.zhiwuduotai.top/gtxpsdbuke.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.guowangkeji.top/gtpnvzeijx.html

[R35] 后台执行并等待
来源：http://hz.bjfxy.top/gtiferpeql.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.hfpthk.cn/gtxpjocmxl.html

[R36] 并发执行多个任务
来源：http://hz.iojbl.cn/gtndmrwnvm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.ydjk.org.cn/gtcrpoqime.html

[R37] 把输出赋给变量
来源：http://hz.52xcode.cn/gtzmavnktb.html

files=$(ls -1)
来源：http://hz.iojbl.cn/gtpjkdrojq.html

[R38] 管道串联
来源：http://hz.iojbl.cn/gtufteblsz.html

cat a.txt | grep -i error | wc -l
来源：http://hz.sweek.top/gtsuybknmm.html

[R39] 重定向标准输出与错误
来源：http://hz.hnxiangtu.top/gtjutxudqf.html

cmd > out.log 2>&1
来源：http://hz.chenjidiqi.icu/gtsrdjcpvx.html

[R40] 追加写日志
来源：http://hz.meibo888.top/gtdxrhcvsn.html

echo "log" >> out.log
来源：http://hz.feifeiyinyue.top/gtsaklbvlk.html

[R41] 丢弃输出
来源：http://hz.ehwqpu.com/gtbvhutkbq.html

cmd >/dev/null 2>&1
来源：http://hz.ppjwa.cn/gtlsypzoyq.html

[R42] 输入重定向
来源：http://hz.yueranfly.top/gtvkzwyknx.html

wc -l < a.txt
来源：http://hz.0kj1m.cn/gtladmdmrs.html

[R43] 按名字查找文件
来源：http://hz.bjfxy.top/gtaxfyfiyj.html

find . -name "*.log" -type f
来源：http://hz.nanxinkj.top/gtnnoruznz.html

[R44] 按修改时间查找
来源：http://hz.xziqi.cn/gtjoitpmgz.html

find . -mtime -7 -type f
来源：http://hz.kuanghao11.cn/gtzcchfrpx.html

[R45] 批量删除
来源：http://hz.jinqigfzy.top/gtxohucnod.html

find . -name "*.tmp" -delete
来源：http://hz.dashuyun.cn/gtzzkmmvkq.html

[R46] 递归替换文件内容
来源：http://hz.jlsjyb.cn/gtdqzeplro.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.dashuyun.cn/gtdvfnsxgh.html

[R47] sed 单行替换
来源：http://hz.wangshuangyany.cn/gtubgspncb.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yanxiufei.cn/gtjhexbujr.html

[R48] awk 取指定列
来源：http://hz.316326.xyz/gtmxnckark.html

awk '{print $1, $3}' a.txt
来源：http://hz.zhiwuduotai.top/gtcudgsgpr.html

[R49] awk 带条件
来源：http://hz.jqgfzy.top/gtenijthdi.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yj20258.top/gtjjthxygk.html

[R50] awk 求和
来源：http://hz.iojbl.cn/gtsrxcjgtu.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.aizwys.cn/gtuopvrhtm.html

[R51] 排序去重取前几
来源：http://hz.xuetiantiany.cn/gtvwandgdj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.yvedp.cn/gthwjllvig.html

[R52] 统计行数
来源：http://hz.andypj.xyz/gthxbhtdlj.html

wc -l a.txt
来源：http://hz.xinyue.icu/gtmteglhkc.html

[R53] 查看文件头与实时尾
来源：http://hz.jianghu66.top/gtcbzsofgu.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.shanyushiyangkeji.top/gtqvqokdzx.html

[R54] 比较两个文件
来源：http://hz.cqqwz.cn/gtzjbhrudr.html

diff a.txt b.txt
来源：http://hz.ybcxt.top/gtvydfkgep.html

[R55] 压缩与解压
来源：http://hz.gotoacloud.top/gtxywthdvc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.9152youxi.cn/gttgylfphm.html

[R56] 远程拷贝
来源：http://hz.yvedp.cn/gtmawojtfi.html

scp file user@host:/path/
来源：http://hz.hysaishi.cn/gtkjedlzlk.html

[R57] 远程执行命令
来源：http://hz.chenzaomai.com/gttakrfhps.html

ssh user@host 'uptime'
来源：http://hz.yangfankeji.com/gtxcvpjlvj.html

[R58] 下载文件
来源：http://hz.yj20258888.top/gtgmzvnosn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.cqqwz.cn/gthfnvtcno.html

[R59] 发 POST JSON
来源：http://hz.cashguo.top/gtnzfgtdya.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.zhixingplan.top/gtzwrsrurh.html

[R60] 只看 HTTP 状态码
来源：http://hz.sysykeji.top/gtirkfzebn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.c1oappe.top/gtkdgmpuqw.html

[R61] 磁盘占用
来源：http://hz.yangfankeji.com/gtxbfzmsfn.html

df -h;  du -sh *
来源：http://hz.havefunace.top/gtuggrkiav.html

[R62] 找最占空间的文件
来源：http://hz.daria6918.cn/gtqpvcxcjq.html

du -ah . | sort -rh | head -10
来源：http://hz.guannengcc.top/gtfngmcuiq.html

[R63] 内存与进程
来源：http://hz.shanyushiyangkeji.top/gtoqsjqohr.html

free -h;  ps aux | grep nginx
来源：http://hz.tian-w.cn/gtwqnyfuab.html

[R64] 结束进程
来源：http://hz.hfpthk.cn/gthhivtzzl.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jinqigufen.top/gtgabhylix.html

[R65] 查看端口占用
来源：http://hz.zhixingplan.top/gtoqteqsvk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.zhoulong.xyz/gtmwcyjjma.html

[R66] 定时任务
来源：http://hz.c1oappe.top/gtidklexwe.html

crontab -e;  crontab -l
来源：http://hz.xuetiantiany.cn/gtfentrcng.html

[R67] 生成随机十六进制串
来源：http://hz.gotoacloud.top/gtzjxupjwt.html

openssl rand -hex 16
来源：http://hz.zdqjudy.top/gtjgmormwj.html

[R68] 计算文件校验值
来源：http://hz.iojbl.cn/gtrusswiiq.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yangfankeji.com/gtwayhobxb.html

[R69] 生成随机密码
来源：http://hz.hfpthk.cn/gtlwnxsbms.html

head -c 16 /dev/urandom | base64
来源：http://hz.zhixingplan.top/gtzawqsmci.html

[R70] 时间戳与互转
来源：http://hz.9152youxi.cn/gtwnawebph.html

date +%s;  date -d @1700000000
来源：http://hz.hammf.cn/gtotsvszxj.html

[R71] 日期格式化
来源：http://hz.yanxiufei.cn/gtacshomkl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.mhx1999.top/gtpmfyiwjj.html

[R72] 等待端口就绪
来源：http://hz.xinyue.icu/gtcqxwkkyy.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.gzhubu.top/gtfphzumxw.html

[R73] 分割大日志
来源：http://hz.jqgfzy.top/gtdnbbstst.html

split -l 1000 big.log part_
来源：http://hz.wangdashe.top/gtmucwrjzb.html

[R74] 批量重命名
来源：http://hz.hongshengwenyu.top/gtdclshbwn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.haohaochexian.top/gtpztgzpac.html

[R75] 导出环境变量
来源：http://hz.shanyushiyangtech.top/gtwndojwpc.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.iojbl.cn/gtlbyisqpk.html

[R76] 使用临时文件
来源：http://hz.guannengcc.top/gtnhlcfjei.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.xinyue.icu/gtjdaxxdvq.html

[R77] 读取用户输入
来源：http://hz.hammf.cn/gtnbzndtsy.html

read -rp "请输入: " ans
来源：http://hz.kuanghao11.cn/gtuxujfjlh.html

[R78] 交互式菜单
来源：http://hz.sweek.top/gtoedamwmj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.316326.xyz/gtisecgaec.html

[R79] 解析命令行选项
来源：http://hz.ydjk.org.cn/gtunfcqzif.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yongpay.top/gtbbhtniuj.html

[R80] 查看脚本执行耗时
来源：http://hz.fengsongda.top/gtxbkvpwis.html

time ./run.sh
来源：http://hz.guowangkeji.top/gtszybxfvv.html

================================================================================
来源：http://hz.wangdashe.top/gtvegzidiy.html

S. C / C++ 专题
来源：http://hz.316326.xyz/gtidaiqepo.html

================================================================================
来源：http://hz.fengsongda.top/gthgutxzhe.html

[S01] C：Hello World
来源：http://hz.cashguo.top/gtzcshwxka.html

#include <stdio.h>
来源：http://hz.xziqi.cn/gtbekizguq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.kuanghao11.cn/gtepmiocfk.html

[S02] C：变量与格式化输出
来源：http://hz.yj20258.top/gtucdsgeyt.html

int a = 10; printf("%d\n", a);
来源：http://hz.shuidangran.top/gtwngemmhr.html

[S03] C：读入整数
来源：http://hz.aibaodan.cn/gtoiqaifcw.html

int x; scanf("%d", &x);
来源：http://hz.aibaodan.cn/gtipcjnaiu.html

[S04] C：字符串复制
来源：http://hz.cheryme.top/gtmzmgxnik.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.9152youxi.cn/gtkloljvld.html

[S05] C：字符串长度
来源：http://hz.havefunace.top/gtqstamfcs.html

strlen(s)
来源：http://hz.gogol.net.cn/gtxhcihecg.html

[S06] C：字符串比较
来源：http://hz.yonumen.top/gtahvnguvu.html

strcmp(a, b) == 0
来源：http://hz.daria6918.cn/gtmazkvshf.html

[S07] C：数组遍历求和
来源：http://hz.tanke756.top/gtouwawmzn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.shuidangran.top/gtfnpufeov.html

[S08] C：动态内存分配与释放
来源：http://hz.gzhubu.top/gtwfpkvxga.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.hongshengwenyu.top/gtmkrqsdse.html

[S09] C：结构体定义与初始化
来源：http://hz.sufxvd.cn/gtpcnsyoub.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.0kj1m.cn/gtnhcsifqf.html

[S10] C：指针与解引用
来源：http://hz.hfpthk.cn/gtpfgtozpa.html

int *p = &a;  *p = 5;
来源：http://hz.jqgufenzy.top/gtsmteedfe.html

[S11] C：逐行读文件
来源：http://hz.hywenlv.cn/gtzdhouddv.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.tanke756.top/gttowhywnw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.9152youxi.cn/gtdpnhrhze.html

fclose(f);
来源：http://hz.hnqzz.top/gtbmngrwwt.html

[S12] C：写文件
来源：http://hz.gaohongyu789.top/gthfbhfbfp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.yuxming.cn/gtvnsgcwke.html

[S13] C：宏定义
来源：http://hz.nanxinkj.top/gtjtuuzrxd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.hnxiangtu.top/gtbaopbtgz.html

[S14] C：枚举
来源：http://hz.zdqjudy.top/gtpvtjsnzo.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.andypj.xyz/gtnsgkvbrk.html

[S15] C：类型转换
来源：http://hz.yuxming.cn/gtgvosbmhd.html

(double) a / b
来源：http://hz.xinyue.icu/gtllsvrlbg.html

[S16] C：位操作置位
来源：http://hz.nwbrower.top/gtqrhcgyrt.html

x |= (1 << 3);
来源：http://hz.xuanzx.com/gtuqqkcloh.html

[S17] C：安全拼接字符串
来源：http://hz.sxryk.cn/gtnsniwdmk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.0kj1m.cn/gtwgymeqgs.html

[S18] C：命令行参数
来源：http://hz.xziqi.cn/gtglltjbja.html

int main(int argc, char **argv)
来源：http://hz.zhiwuduotai.top/gtioytovtr.html

[S19] C：快速排序
来源：http://hz.andypj.xyz/gtivffduxi.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yangfankeji.com/gteyiqqbvg.html

[S20] C：二分查找
来源：http://hz.xziqi.cn/gtqbgmmzms.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.jyoumei.cn/gtyboatgxk.html

[S21] C：字符类别判断
来源：http://hz.cashguo.top/gtnqqbtdqu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.feifeiyinyue.top/gtytnhuukt.html

[S22] C：字符串转数字
来源：http://hz.cucudq.cn/gtsqehjnol.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.cheryme.top/gtiwxcmbvc.html

[S23] C：随机数
来源：http://hz.hfpthk.cn/gtswlcagfd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.yuanzhike.top/gtbeftstah.html

[S24] C：获取本地时间
来源：http://hz.haohaochexian.top/gtdptnyhsb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.tian-w.cn/gtqqachvvo.html

[S25] C：内存拷贝
来源：http://hz.jianghu66.top/gtznlwrmpq.html

memcpy(dst, src, n);
来源：http://hz.tian-w.cn/gtinkqrqow.html

[S26] C：内存清零
来源：http://hz.shangyingyoupin.top/gttrzeszax.html

memset(a, 0, sizeof a);
来源：http://hz.xuanzx.com/gttudrdbdi.html

[S27] C：定义常量
来源：http://hz.gzhubu.top/gtgbsacouu.html

const double PI = 3.14159;
来源：http://hz.pycfn.com/gtzlodzhoq.html

[S28] C：静态变量
来源：http://hz.smart0.xyz/gtfbmglhob.html

static int counter = 0;
来源：http://hz.hysaishi.cn/gtgxazdpvx.html

[S29] C：变参函数
来源：http://hz.hysaishi.cn/gtxdyatevl.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.sufxvd.cn/gtvyihhmlo.html

[S30] C：头文件保护
来源：http://hz.hywenlv.cn/gtfkekqriq.html

#ifndef X_H
来源：http://hz.cucudq.cn/gtdyegycvk.html

#define X_H
来源：http://hz.0kj1m.cn/gtbcfujdhv.html

#endif
来源：http://hz.quarkkingdee.top/gttnkobral.html

[S31] C++：Hello World
来源：http://hz.jqgfzy.top/gtsbqhejtq.html

#include <iostream>
来源：http://hz.shzxlz.cn/gtypfqqpas.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.zhengqikj.top/gtislwhvfj.html

[S32] C++：字符串
来源：http://hz.pengpengdd.cyou/gtazkxzybs.html

std::string s = "hi";  s += "!";
来源：http://hz.sweek.top/gtainaqsnf.html

[S33] C++：vector 增删
来源：http://hz.aizwys.cn/gtxodfnnca.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.kuanghao11.cn/gtcicoiaws.html

[S34] C++：遍历 vector
来源：http://hz.jinyuanbaomall.cn/gtayaukbuq.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.iojbl.cn/gtuieowmaa.html

[S35] C++：map
来源：http://hz.ppjwa.cn/gtpqhtonrx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.316326.xyz/gtnoshtqza.html

[S36] C++：unordered_map
来源：http://hz.ydzc1.top/gtppduuknu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.wangshuangyany.cn/gtasuwzyab.html

[S37] C++：set
来源：http://hz.ydzc1.top/gtlrwwgkpa.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.chenzaomai.com/gtckezhvjp.html

[S38] C++：排序
来源：http://hz.shanyushiyangtech.top/gtufnvvhnj.html

std::sort(v.begin(), v.end());
来源：http://hz.guowangkeji.top/gtuwkbnygo.html

[S39] C++：自定义比较器排序
来源：http://hz.yangfankeji.com/gtweeqwpao.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.tianlin.xyz/gtpbennwpp.html

[S40] C++：查找元素
来源：http://hz.gaohongyu789.top/gtfkwnfwxt.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.meibo888.top/gtkvhicaxg.html

[S41] C++：类与构造函数
来源：http://hz.jinghuilouyu.cn/gtxtrvlubs.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.feifeiyinyue.top/gtjnxibtnh.html

[S42] C++：继承与虚函数
来源：http://hz.snrcjt.cn/gtsjfzomrk.html

class B : public Base { public: void f() override {} };
来源：http://hz.0kj1m.cn/gtyhlkdzyj.html

[S43] C++：智能指针
来源：http://hz.xinyue.icu/gtxkeeugyl.html

auto p = std::make_unique<int>(5);
来源：http://hz.jqgfzy.top/gtctcievde.html

[S44] C++：引用传参
来源：http://hz.xinyue.icu/gtwzcsschd.html

void inc(int &x) { ++x; }
来源：http://hz.meibo888.top/gtaisgjheb.html

[S45] C++：lambda
来源：http://hz.kuanghao11.cn/gtyzdrnmic.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.snrcjt.cn/gtmxintgsv.html

[S46] C++：函数模板
来源：http://hz.quarkkingdee.top/gtwungpzbg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.quarkkingdee.top/gtidyxglnb.html

[S47] C++：结构化绑定遍历
来源：http://hz.xylfe.cn/gtkexlklhm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.zhengqikj.top/gtpddglulp.html

[S48] C++：逐行读文件
来源：http://hz.52xcode.cn/gtoivkayri.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.c1oappe.top/gtfleflxjf.html

while (std::getline(in, line)) { }
来源：http://hz.chenjidiqi.icu/gttmufrxho.html

[S49] C++：写文件
来源：http://hz.jyoumei.cn/gtjxydebop.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.aizwys.cn/gthgqncksb.html

[S50] C++：格式化数字
来源：http://hz.kuanghao11.cn/gtouvzvsqw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.cdnleiting.top/gtkyfswxme.html

[S51] C++：显式类型转换
来源：http://hz.hnqzz.top/gtpnzfpnvq.html

static_cast<double>(a) / b
来源：http://hz.shanyushiyangkeji.top/gtrsfmgpba.html

[S52] C++：const 与 noexcept
来源：http://hz.cqqwz.cn/gtkukwpzuj.html

int size() const noexcept { return n_; }
来源：http://hz.52xcode.cn/gtjqjeegbh.html

[S53] C++：移动语义
来源：http://hz.quarkkingdee.top/gtigetdpmq.html

std::vector<int> w = std::move(v);
来源：http://hz.yj20258.top/gtqlekteud.html

[S54] C++：异常处理
来源：http://hz.hywenlv.cn/gtlvpvmtgv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.kuanghao11.cn/gtzsrnsxjw.html

[S55] C++：结构化绑定
来源：http://hz.xziqi.cn/gtutunpypu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.xuanzx.com/gtygqxuqtz.html

[S56] C++：optional
来源：http://hz.0kj1m.cn/gtvasnuycj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.xinyue.icu/gtgkuzcgxo.html

[S57] C++：编译期常量
来源：http://hz.svipenyu.cn/gtppuzgsfs.html

constexpr int N = 10;
来源：http://hz.cucudq.cn/gtrydqcvll.html

[S58] C++：命名空间
来源：http://hz.svipenyu.cn/gtumialpnh.html

namespace ns { int f() { return 1; } }
来源：http://hz.tianlin.xyz/gtoqddkvwp.html

[S59] C++：静态断言
来源：http://hz.hnxiangtu.top/gtfzlahcvg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.0kj1m.cn/gteotxehmf.html

[S60] C++：遍历并删除元素
来源：http://hz.gaohongyu789.top/gtxixwbslp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yongpay.top/gtlpqxiznr.html

================================================================================
来源：http://hz.yangfankeji.com/gtcvdffsiz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.wangdashe.top/gtexaaogeu.html

================================================================================
来源：http://hz.52xcode.cn/gtyaiptwoc.html

[T01] Kotlin：Hello World
来源：http://hz.ydjk.org.cn/gtmyfbaoad.html

println("Hello")
来源：http://hz.yanxiufei.cn/gtzwkyibcq.html

[T02] Kotlin：变量
来源：http://hz.mhx1999.top/gtjyzzsswd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.shzxlz.cn/gtgwybmvcg.html

[T03] Kotlin：字符串模板
来源：http://hz.andypj.xyz/gtswtzdabp.html

"值: $b"
来源：http://hz.fzhhl.top/gtecciwqch.html

[T04] Kotlin：空安全
来源：http://hz.shanyushiyangkeji.top/gttxlepysh.html

val n: String? = null;  n?.length
来源：http://hz.hnxiangtu.top/gtcvdkfnbe.html

[T05] Kotlin：when 表达式
来源：http://hz.zycfv.cn/gtxigmwowm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yvedp.cn/gtaikarkpc.html

[T06] Kotlin：集合映射
来源：http://hz.zhijiandao.cn/gtgbjserev.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.zhixingplan.top/gtnnmqixcb.html

[T07] Kotlin：集合过滤
来源：http://hz.cucudq.cn/gtcysgtasi.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.xinyue.icu/gtncejawxb.html

[T08] Kotlin：数据类
来源：http://hz.haohaochexian.top/gtamiwigxz.html

data class User(val name: String, val age: Int)
来源：http://hz.quarkkingdee.top/gtmjdbkmww.html

[T09] Kotlin：扩展函数
来源：http://hz.quarkkingdee.top/gtgbaqnwkz.html

fun String.exclaim() = this + "!"
来源：http://hz.yongpay.top/gtzxdfofyo.html

[T10] Kotlin：默认参数
来源：http://hz.9152youxi.cn/gtvkjzdgvz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.gogol.net.cn/gtcudzsyqj.html


<!-- 参考信息 -->