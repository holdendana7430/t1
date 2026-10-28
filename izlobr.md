代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.xylfe.cn/gtarepfqrr.html

[R10] 正则匹配
来源：http://hz.hywenlv.cn/gtwskqyvwo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.gotoacloud.top/gtowmlekbr.html

[R11] case 多分支
来源：http://hz.guannengcc.top/gtnxyxjmcq.html

case "$1" in
来源：http://hz.xylfe.cn/gtvjfjhqzy.html

start) echo "启动" ;;
来源：http://hz.fengsongda.top/gtrmwiusrz.html

stop)  echo "停止" ;;
来源：http://hz.ydjk.org.cn/gtzrfkrrqx.html

*)     echo "未知命令" ;;
来源：http://hz.zhaomingkeji.xyz/gtmxlfihii.html

esac
来源：http://hz.chenzaomai.com/gtcwxunuma.html

[R12] for 遍历文件
来源：http://hz.hnxiangtu.top/gtzuenebfg.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jqgfzy.top/gtlqyqcgvt.html

[R13] for 计数循环
来源：http://hz.ywan-chungtsiang.top/gtvntrhtdu.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.shanyushiyangkeji.top/gtdhcoezpt.html

[R14] C 风格 for
来源：http://hz.yuxming.cn/gtvwezaain.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jinqigfzy.top/gtwnqsobmt.html

[R15] while 逐行读文件
来源：http://hz.zhijiandao.cn/gtngizmeop.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yj20258888.top/gtptmwbzxb.html

[R16] until 等待条件
来源：http://hz.wangdashe.top/gtqdbocxpb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yj20258888.top/gtyibhsvur.html

[R17] 数组定义与取值
来源：http://hz.quarkkingdee.top/gtfsomnvkc.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.shuidangran.top/gtishkpunn.html

[R18] 遍历数组
来源：http://hz.sxryk.cn/gtujnpfnlu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.sweek.top/gtvqvzyvhk.html

[R19] 数组长度
来源：http://hz.xuetiantiany.cn/gtepkyksuv.html

echo "${#arr[@]}"
来源：http://hz.shangyingyoupin.top/gtihqiitvo.html

[R20] 关联数组（字典）
来源：http://hz.jinghuilouyu.cn/gtdklixwfv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zhixingplan.top/gttqsmeyos.html

[R21] 字符串长度
来源：http://hz.yj20258888.top/gtnbmqlejp.html

echo "${#s}"
来源：http://hz.zycfv.cn/gtiiszjofl.html

[R22] 截取子串
来源：http://hz.chenjidiqi.icu/gtylhusjyu.html

echo "${s:0:5}"
来源：http://hz.zhiwuduotai.top/gtmlrepsom.html

[R23] 字符串替换
来源：http://hz.iojbl.cn/gtspgqonib.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.cucudq.cn/gtutmtland.html

[R24] 大小写转换
来源：http://hz.hfpthk.cn/gtyoqyyrkr.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.zhijiandao.cn/gtgdkznmfa.html

[R25] 去后缀 / 去前缀
来源：http://hz.sysykeji.top/gtspfmzcph.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.dashuyun.cn/gtdebbinmj.html

[R26] 命令替换
来源：http://hz.sweek.top/gtdshqpmwf.html

now=$(date +%F); echo "$now"
来源：http://hz.zhixingplan.top/gtbdkjspcb.html

[R27] 算术展开
来源：http://hz.gzhubu.top/gtvslisfsc.html

echo $((1 + 2 * 3))
来源：http://hz.gogol.net.cn/gtgvofchgy.html

[R28] 浮点运算
来源：http://hz.chenlongwang.top/gtaznwnrsv.html

echo "scale=2; 10/3" | bc
来源：http://hz.tanke756.top/gtzdkeksfs.html

[R29] 定义函数
来源：http://hz.zhixingplan.top/gtfjietfas.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.hysaishi.cn/gtphuziwwe.html

[R30] 函数返回状态码
来源：http://hz.vqdsnc.cn/gtohrsargh.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jqgufenzy.top/gtigqzboks.html

[R31] 局部变量
来源：http://hz.zdqjudy.top/gtvhsqfjhk.html

f() { local x=1; echo "$x"; }
来源：http://hz.ydjk.org.cn/gtbbnylkfp.html

[R32] 参数个数校验
来源：http://hz.shanyushiyangkeji.top/gtldcohzhq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.xuanzx.com/gtqtnhmbhp.html

[R33] 捕获错误并提示行号
来源：http://hz.jyoumei.cn/gtupueblud.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zdqjudy.top/gtmkgknxiz.html

[R34] 退出时清理
来源：http://hz.zycfv.cn/gtpzkesttx.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.wangdashe.top/gtwgyjqmko.html

[R35] 后台执行并等待
来源：http://hz.jyoumei.cn/gtqlqxphao.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yonumen.top/gtllhufhds.html

[R36] 并发执行多个任务
来源：http://hz.zhiwuduotai.top/gtdplbswjl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.cdnleiting.top/gtvvfankod.html

[R37] 把输出赋给变量
来源：http://hz.ydjk.org.cn/gtenvdfdkb.html

files=$(ls -1)
来源：http://hz.daxiang520.top/gtsuewbrjg.html

[R38] 管道串联
来源：http://hz.jinqigfzy.top/gtevdjgldf.html

cat a.txt | grep -i error | wc -l
来源：http://hz.wangdashe.top/gtzcspxjne.html

[R39] 重定向标准输出与错误
来源：http://hz.jiagoushi.top/gtxjnsngwc.html

cmd > out.log 2>&1
来源：http://hz.jqgfzy.top/gtytoagsuf.html

[R40] 追加写日志
来源：http://hz.mhx1999.top/gtnweufhax.html

echo "log" >> out.log
来源：http://hz.ybcxt.top/gtecmulepq.html

[R41] 丢弃输出
来源：http://hz.dashuyun.cn/gtpbezenvg.html

cmd >/dev/null 2>&1
来源：http://hz.xinyue.icu/gtytqvmtuh.html

[R42] 输入重定向
来源：http://hz.gaohongyu789.top/gtrrenunqu.html

wc -l < a.txt
来源：http://hz.guowangkeji.top/gtauvspptb.html

[R43] 按名字查找文件
来源：http://hz.jiagoushi.top/gtycmbcmrt.html

find . -name "*.log" -type f
来源：http://hz.yvedp.cn/gtwlhydlxw.html

[R44] 按修改时间查找
来源：http://hz.zycfv.cn/gtyhfpbkus.html

find . -mtime -7 -type f
来源：http://hz.zhaomingkeji.xyz/gtkoifssqk.html

[R45] 批量删除
来源：http://hz.kuanghao11.cn/gtyfmaueet.html

find . -name "*.tmp" -delete
来源：http://hz.jinqigfzy.top/gtozidmjqk.html

[R46] 递归替换文件内容
来源：http://hz.316326.xyz/gtcymoidjx.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.andypj.xyz/gtnzagxkrv.html

[R47] sed 单行替换
来源：http://hz.yj202588.top/gttmvxwyyz.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.daria6918.cn/gtzbtcymxx.html

[R48] awk 取指定列
来源：http://hz.ehwqpu.com/gtrzqnywwx.html

awk '{print $1, $3}' a.txt
来源：http://hz.hnqzz.top/gtovtcltox.html

[R49] awk 带条件
来源：http://hz.sufxvd.cn/gtsejmqjva.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.jinqigfzy.top/gtsdcxyqay.html

[R50] awk 求和
来源：http://hz.cdnleiting.top/gtybdrxzkw.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.nanxuanxn.top/gtewzhnyld.html

[R51] 排序去重取前几
来源：http://hz.zhixingplan.top/gtaotonukw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.andypj.xyz/gtykiuemuq.html

[R52] 统计行数
来源：http://hz.yueranfly.top/gtjchpedkm.html

wc -l a.txt
来源：http://hz.xziqi.cn/gtbigmqykg.html

[R53] 查看文件头与实时尾
来源：http://hz.gotoacloud.top/gtdrbiccaj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.zhengqikj.top/gtmsltkexl.html

[R54] 比较两个文件
来源：http://hz.sxryk.cn/gtrakiiwnr.html

diff a.txt b.txt
来源：http://hz.cucudq.cn/gtuasuicfk.html

[R55] 压缩与解压
来源：http://hz.zhaomingkeji.xyz/gttvduiqpg.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.hongshengwenyu.top/gtgdaqvatg.html

[R56] 远程拷贝
来源：http://hz.jinqigfzy.top/gtevodofri.html

scp file user@host:/path/
来源：http://hz.yj20258888.top/gtceqthkex.html

[R57] 远程执行命令
来源：http://hz.0kj1m.cn/gtdkcejqgc.html

ssh user@host 'uptime'
来源：http://hz.xinyue.icu/gtwexgthtl.html

[R58] 下载文件
来源：http://hz.nanxuanxn.top/gtrfmyhibc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.52xcode.cn/gtgqcenpcr.html

[R59] 发 POST JSON
来源：http://hz.tian-w.cn/gtbxtfrahy.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.guannengcc.top/gtgwljplya.html

[R60] 只看 HTTP 状态码
来源：http://hz.dianchejie.cn/gtzlgezfgo.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.aizwys.cn/gtouxyxkhj.html

[R61] 磁盘占用
来源：http://hz.pengpengdd.cyou/gtgauwztba.html

df -h;  du -sh *
来源：http://hz.hammf.cn/gtwkhxyvnx.html

[R62] 找最占空间的文件
来源：http://hz.shanyushiyangtech.top/gttmcgdwnq.html

du -ah . | sort -rh | head -10
来源：http://hz.zhiwuduotai.top/gtrazbulkw.html

[R63] 内存与进程
来源：http://hz.xziqi.cn/gtdczukzjl.html

free -h;  ps aux | grep nginx
来源：http://hz.ybcxt.top/gtresmgbzd.html

[R64] 结束进程
来源：http://hz.aizwys.cn/gtfonofdee.html

kill -9 $(pgrep -f app.py)
来源：http://hz.zhongyouzk.top/gtcawfzkey.html

[R65] 查看端口占用
来源：http://hz.yongpay.top/gtowcmfajl.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.ivvv.top/gtubgulkjg.html

[R66] 定时任务
来源：http://hz.vqdsnc.cn/gtwmbakgwo.html

crontab -e;  crontab -l
来源：http://hz.cqqwz.cn/gtmjajminl.html

[R67] 生成随机十六进制串
来源：http://hz.daxiang520.top/gturiypnqe.html

openssl rand -hex 16
来源：http://hz.jlsjyb.cn/gtmswgfcag.html

[R68] 计算文件校验值
来源：http://hz.sweek.top/gtqcljanuu.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.zycfv.cn/gtidkgfodu.html

[R69] 生成随机密码
来源：http://hz.mhx1999.top/gtahztfpgz.html

head -c 16 /dev/urandom | base64
来源：http://hz.gotoacloud.top/gturdrkxtn.html

[R70] 时间戳与互转
来源：http://hz.zhengqikj.top/gtoubeeyic.html

date +%s;  date -d @1700000000
来源：http://hz.xuetiantiany.cn/gtrfsllcwy.html

[R71] 日期格式化
来源：http://hz.9152youxi.cn/gtlhwwoupd.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.sufxvd.cn/gthskzijzi.html

[R72] 等待端口就绪
来源：http://hz.yongpay.top/gtajqebnxx.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.shanyushiyangtech.top/gtudmkhble.html

[R73] 分割大日志
来源：http://hz.yj202588.top/gtqjglilrh.html

split -l 1000 big.log part_
来源：http://hz.hnqzz.top/gtwlswsgai.html

[R74] 批量重命名
来源：http://hz.ydzc1.top/gtienblldl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.tanke756.top/gtzjeqonow.html

[R75] 导出环境变量
来源：http://hz.ppjwa.cn/gtkbxbpjyk.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.9152youxi.cn/gtncqccvpx.html

[R76] 使用临时文件
来源：http://hz.havefunace.top/gtwxzngkhi.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.chenjidiqi.icu/gtyjxvivwv.html

[R77] 读取用户输入
来源：http://hz.aibaodan.cn/gtvmlrbldi.html

read -rp "请输入: " ans
来源：http://hz.fzhhl.top/gtshnvzcka.html

[R78] 交互式菜单
来源：http://hz.ydzc1.top/gtrdgpelcu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.ydzc1.top/gtcgnugerq.html

[R79] 解析命令行选项
来源：http://hz.yueranfly.top/gtojmmpypm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.sweek.top/gtxjrexocd.html

[R80] 查看脚本执行耗时
来源：http://hz.iojbl.cn/gtqwywsckg.html

time ./run.sh
来源：http://hz.pycfn.com/gtwnewtolw.html

================================================================================
来源：http://hz.ehwqpu.com/gtgifgxiub.html

S. C / C++ 专题
来源：http://hz.yj20258.top/gtonjcedrr.html

================================================================================
来源：http://hz.yanxiufei.cn/gtfshtlael.html

[S01] C：Hello World
来源：http://hz.havefunace.top/gtmfunsbws.html

#include <stdio.h>
来源：http://hz.zycfv.cn/gtoqryinob.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jinqigufen.top/gtvkqksbyg.html

[S02] C：变量与格式化输出
来源：http://hz.sweek.top/gtsgsrgwwm.html

int a = 10; printf("%d\n", a);
来源：http://hz.chenzaomai.com/gtdhcwwkeu.html

[S03] C：读入整数
来源：http://hz.yanxiufei.cn/gtmdcwqrgc.html

int x; scanf("%d", &x);
来源：http://hz.feifeiyinyue.top/gtrqbwmgqt.html

[S04] C：字符串复制
来源：http://hz.zhixingplan.top/gtachonozi.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.xziqi.cn/gtudwnhlyc.html

[S05] C：字符串长度
来源：http://hz.zhiwuduotai.top/gtbvmwsalf.html

strlen(s)
来源：http://hz.dashuyun.cn/gttmelzhdl.html

[S06] C：字符串比较
来源：http://hz.shanyushiyangkeji.top/gtasxrdlnu.html

strcmp(a, b) == 0
来源：http://hz.quarkkingdee.top/gtkvwqtiig.html

[S07] C：数组遍历求和
来源：http://hz.quarkkingdee.top/gtdnubmpqb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.svipenyu.cn/gtdeaqpiqq.html

[S08] C：动态内存分配与释放
来源：http://hz.ppjwa.cn/gtygmwmebu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.shangyingyoupin.top/gtidxhprez.html

[S09] C：结构体定义与初始化
来源：http://hz.aizwys.cn/gtrhohkfpc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.c1oappe.top/gtcliujmxw.html

[S10] C：指针与解引用
来源：http://hz.chenlongwang.top/gtcdgpuvun.html

int *p = &a;  *p = 5;
来源：http://hz.jinyuanbaomall.cn/gtxcshuhao.html

[S11] C：逐行读文件
来源：http://hz.andypj.xyz/gtuupkhjbw.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.smart0.xyz/gtieymyhxs.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.nanxuanxn.top/gtyfljlhcw.html

fclose(f);
来源：http://hz.sysykeji.top/gtdxbgtxqz.html

[S12] C：写文件
来源：http://hz.svipenyu.cn/gtsjkkofzi.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.hnqzz.top/gtvdvwrpry.html

[S13] C：宏定义
来源：http://hz.shzxlz.cn/gtdazcsyji.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.svipenyu.cn/gthwartoxh.html

[S14] C：枚举
来源：http://hz.guannengcc.top/gtaxzpbzqu.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.jlsjyb.cn/gtxutflycv.html

[S15] C：类型转换
来源：http://hz.ybcxt.top/gtcpbfsagk.html

(double) a / b
来源：http://hz.gaohongyu789.top/gtlqevaapz.html

[S16] C：位操作置位
来源：http://hz.yj20258.top/gtduidveli.html

x |= (1 << 3);
来源：http://hz.sweek.top/gtnmuitzqw.html

[S17] C：安全拼接字符串
来源：http://hz.zhijiandao.cn/gtvucdytxy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.haohaochexian.top/gtydybfshf.html

[S18] C：命令行参数
来源：http://hz.iojbl.cn/gtyjxhogck.html

int main(int argc, char **argv)
来源：http://hz.yanxiufei.cn/gtsfqvmbiz.html

[S19] C：快速排序
来源：http://hz.xinyue.icu/gtgcymfqnd.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.haohaochexian.top/gtwrwxkkac.html

[S20] C：二分查找
来源：http://hz.zhijiandao.cn/gtftmiblqn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.jianghu66.top/gtfmyattog.html

[S21] C：字符类别判断
来源：http://hz.316326.xyz/gtfyrjxamu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.52xcode.cn/gtkeoyigya.html

[S22] C：字符串转数字
来源：http://hz.0kj1m.cn/gtijscgdgg.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.bjfxy.top/gtnxltuwkl.html

[S23] C：随机数
来源：http://hz.meibo888.top/gtvkyefzzk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.smart0.xyz/gtrfpckakj.html

[S24] C：获取本地时间
来源：http://hz.sweek.top/gtqavlqflj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.ppjwa.cn/gtebvjdzho.html

[S25] C：内存拷贝
来源：http://hz.mhx1999.top/gtlttankux.html

memcpy(dst, src, n);
来源：http://hz.hywenlv.cn/gtjobwhvlb.html

[S26] C：内存清零
来源：http://hz.feifeiyinyue.top/gtmmiwdssb.html

memset(a, 0, sizeof a);
来源：http://hz.tanke756.top/gtiskcyojb.html

[S27] C：定义常量
来源：http://hz.quarkkingdee.top/gtabdxigyn.html

const double PI = 3.14159;
来源：http://hz.xylfe.cn/gthkwnutdd.html

[S28] C：静态变量
来源：http://hz.yuxming.cn/gtnugwthcu.html

static int counter = 0;
来源：http://hz.yangfankeji.com/gtjzobkotp.html

[S29] C：变参函数
来源：http://hz.0kj1m.cn/gtgaiyxbfh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.yangfankeji.com/gtrubhjorp.html

[S30] C：头文件保护
来源：http://hz.jiagoushi.top/gtpvtboesw.html

#ifndef X_H
来源：http://hz.shangyingyoupin.top/gtgnnfwfvy.html

#define X_H
来源：http://hz.ydzc1.top/gtbyvdlvjb.html

#endif
来源：http://hz.cashguo.top/gtctuuudnq.html

[S31] C++：Hello World
来源：http://hz.52xcode.cn/gtvatihalr.html

#include <iostream>
来源：http://hz.jyoumei.cn/gttlstnfyh.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.xylfe.cn/gtyzfshqnc.html

[S32] C++：字符串
来源：http://hz.zdqjudy.top/gthpwcnnza.html

std::string s = "hi";  s += "!";
来源：http://hz.svipenyu.cn/gthekuwytf.html

[S33] C++：vector 增删
来源：http://hz.zhengqikj.top/gtilpqeibg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.fengsongda.top/gtxplcdmeb.html

[S34] C++：遍历 vector
来源：http://hz.9152youxi.cn/gtymfmlcni.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.zhijiandao.cn/gtecunllwl.html

[S35] C++：map
来源：http://hz.zhixingplan.top/gtjydgebpz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xingfuxueyuan.xyz/gtjgckxscz.html

[S36] C++：unordered_map
来源：http://hz.jiagoushi.top/gtuexrcysn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.haohaochexian.top/gtxqjlcuez.html

[S37] C++：set
来源：http://hz.kuanghao11.cn/gtiqoqjgaq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.bjfxy.top/gtickbjiuq.html

[S38] C++：排序
来源：http://hz.hfpthk.cn/gthkqpfnxd.html

std::sort(v.begin(), v.end());
来源：http://hz.yj202588.top/gtggwjqekb.html

[S39] C++：自定义比较器排序
来源：http://hz.cdnleiting.top/gtmaedwynj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.fengsongda.top/gtubxiuxih.html

[S40] C++：查找元素
来源：http://hz.andypj.xyz/gtmwpwmzis.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.xziqi.cn/gtccrcodoo.html

[S41] C++：类与构造函数
来源：http://hz.xziqi.cn/gtdmmnypdx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.shanyushiyangkeji.top/gtmgryvncy.html

[S42] C++：继承与虚函数
来源：http://hz.chenzaomai.com/gtvgrrsqka.html

class B : public Base { public: void f() override {} };
来源：http://hz.daria6918.cn/gtaktsegqc.html

[S43] C++：智能指针
来源：http://hz.daxiang520.top/gtagqrjfbc.html

auto p = std::make_unique<int>(5);
来源：http://hz.ivvv.top/gtvehqtxvr.html

[S44] C++：引用传参
来源：http://hz.aibaodan.cn/gtwycueybv.html

void inc(int &x) { ++x; }
来源：http://hz.ehwqpu.com/gtilbipjpb.html

[S45] C++：lambda
来源：http://hz.snrcjt.cn/gthiausaai.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.nanxuanxn.top/gtisdiwtmo.html

[S46] C++：函数模板
来源：http://hz.hnxiangtu.top/gtuknzcofu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yangfankeji.com/gtqdwnltbi.html

[S47] C++：结构化绑定遍历
来源：http://hz.sxryk.cn/gtwhrbrqro.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.cucudq.cn/gtwdzrejmf.html

[S48] C++：逐行读文件
来源：http://hz.ydjk.org.cn/gtuneaptan.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yj202588.top/gtigloqwzr.html

while (std::getline(in, line)) { }
来源：http://hz.pengpengdd.cyou/gtxfaekzoz.html

[S49] C++：写文件
来源：http://hz.bjfxy.top/gtvxadgetz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.xingfuxueyuan.xyz/gtjowdtbcn.html

[S50] C++：格式化数字
来源：http://hz.zdqjudy.top/gtlxcdalrm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.fzhhl.top/gtbghwazew.html

[S51] C++：显式类型转换
来源：http://hz.zdqjudy.top/gtbzqmaapj.html

static_cast<double>(a) / b
来源：http://hz.chenjidiqi.icu/gtydqwfwfh.html

[S52] C++：const 与 noexcept
来源：http://hz.tanke756.top/gtzelpuhso.html

int size() const noexcept { return n_; }
来源：http://hz.jqgufenzy.top/gtpxvvpzyn.html

[S53] C++：移动语义
来源：http://hz.haohaochexian.top/gthlmqkciv.html

std::vector<int> w = std::move(v);
来源：http://hz.shanyushiyangtech.top/gtqqpgvhog.html

[S54] C++：异常处理
来源：http://hz.jinqigufen.top/gtnxavlrws.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.feifeiyinyue.top/gtnslmedlz.html

[S55] C++：结构化绑定
来源：http://hz.chenzaomai.com/gtaodjpehh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.sufxvd.cn/gtiunhztiu.html

[S56] C++：optional
来源：http://hz.ivvv.top/gtwzvawxmv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.hongshengwenyu.top/gtihdwqkla.html

[S57] C++：编译期常量
来源：http://hz.zdqjudy.top/gtmpqgfuap.html

constexpr int N = 10;
来源：http://hz.shuidangran.top/gtsqnqsefr.html

[S58] C++：命名空间
来源：http://hz.cheryme.top/gtvloggijd.html

namespace ns { int f() { return 1; } }
来源：http://hz.shangyingyoupin.top/gtcticoerk.html

[S59] C++：静态断言
来源：http://hz.jqgufenzy.top/gtoqzpdnwf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.yonumen.top/gtveqtiowx.html

[S60] C++：遍历并删除元素
来源：http://hz.yj20258888.top/gtpcijcczq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.nanxinkj.top/gtmfolxbpa.html

================================================================================
来源：http://hz.svipenyu.cn/gtydpuxskf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.pengpengdd.cyou/gtkldnhcdj.html

================================================================================
来源：http://hz.ehwqpu.com/gtczrjkzco.html

[T01] Kotlin：Hello World
来源：http://hz.ydzc1.top/gtfrrubath.html

println("Hello")
来源：http://hz.gotoacloud.top/gtzkrnzmvv.html

[T02] Kotlin：变量
来源：http://hz.fengsongda.top/gtbmsadmnj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.bjfxy.top/gtflmlvczy.html

[T03] Kotlin：字符串模板
来源：http://hz.yj202588.top/gtfregdwgd.html

"值: $b"
来源：http://hz.nwbrower.top/gtjnsxlvdb.html

[T04] Kotlin：空安全
来源：http://hz.redwolf501.top/gtfmoswxfc.html

val n: String? = null;  n?.length
来源：http://hz.gogol.net.cn/gtvcnmdeab.html

[T05] Kotlin：when 表达式
来源：http://hz.gaohongyu789.top/gtoyisievz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.vqdsnc.cn/gtcfbimnyg.html

[T06] Kotlin：集合映射
来源：http://hz.fzhhl.top/gtydmzkrhr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.guannengcc.top/gthvgoyylk.html

[T07] Kotlin：集合过滤
来源：http://hz.haohaochexian.top/gtmthyiykl.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.ivvv.top/gtcwmfmzyk.html

[T08] Kotlin：数据类
来源：http://hz.jqgfzy.top/gtxpmniswl.html

data class User(val name: String, val age: Int)
来源：http://hz.hnqzz.top/gtlormkncq.html

[T09] Kotlin：扩展函数
来源：http://hz.yj20258.top/gtectlqekv.html

fun String.exclaim() = this + "!"
来源：http://hz.daria6918.cn/gtfhjcrlwk.html

[T10] Kotlin：默认参数
来源：http://hz.yongpay.top/gtivyjqfev.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.guannengcc.top/gtrvvkbtvf.html


<!-- 参考信息 -->