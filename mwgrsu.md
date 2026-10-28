代发 wailian999

readonly PI=3.14
来源：http://hz.zhaomingkeji.xyz/gtdtduxpiv.html

[R04] 位置参数
来源：http://hz.aizwys.cn/gtqfrjmvkd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.ydzc1.top/gtkugaiplw.html

[R05] 参数默认值
来源：http://hz.ybcxt.top/gtstnfniml.html

name="${1:-default}"
来源：http://hz.xinyue.icu/gtbwselote.html

[R06] 判断命令是否存在
来源：http://hz.dashuyun.cn/gtdtrncsib.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yangfankeji.com/gtvuhkrfut.html

[R07] if 判断文件
来源：http://hz.smart0.xyz/gtuslgmiob.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.birdmap.top/gtjhnwboiq.html

[R08] 数值比较
来源：http://hz.nanxinkj.top/gtbcvjizcb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.kuanghao11.cn/gtxfyitoum.html

[R09] 字符串比较
来源：http://hz.ehwqpu.com/gtkrcsjjsf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zhengqikj.top/gtswpjyrxw.html

[R10] 正则匹配
来源：http://hz.xylfe.cn/gtezhmcvvy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.gogol.net.cn/gtvietzhso.html

[R11] case 多分支
来源：http://hz.nanxuanxn.top/gtogkmlset.html

case "$1" in
来源：http://hz.fengsongda.top/gtrkmjlcso.html

start) echo "启动" ;;
来源：http://hz.wangshuangyany.cn/gtraswfzsl.html

stop)  echo "停止" ;;
来源：http://hz.chenlongwang.top/gtrhrjhqgr.html

*)     echo "未知命令" ;;
来源：http://hz.wangdashe.top/gtriejbsxd.html

esac
来源：http://hz.havefunace.top/gtstrpzwdf.html

[R12] for 遍历文件
来源：http://hz.jqgfzy.top/gtrcrsmgri.html

for f in *.txt; do echo "$f"; done
来源：http://hz.zhengqikj.top/gtcntxebxe.html

[R13] for 计数循环
来源：http://hz.hfpthk.cn/gtmqaubset.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.xuanzx.com/gtriyxbzxf.html

[R14] C 风格 for
来源：http://hz.xuetiantiany.cn/gthlytntpp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jqgufenzy.top/gtbnytkypg.html

[R15] while 逐行读文件
来源：http://hz.yj202588.top/gtqwxghgof.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.cheryme.top/gtyquuvnwk.html

[R16] until 等待条件
来源：http://hz.sweek.top/gtdcwfjdsj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.gaohongyu789.top/gthorpppfj.html

[R17] 数组定义与取值
来源：http://hz.cqqwz.cn/gtslajsoir.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yanxiufei.cn/gtpbcuzohm.html

[R18] 遍历数组
来源：http://hz.xuanzx.com/gtkfioaxog.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.hongshengwenyu.top/gtcyufriiq.html

[R19] 数组长度
来源：http://hz.zhijiandao.cn/gtlmdkrhmv.html

echo "${#arr[@]}"
来源：http://hz.ywan-chungtsiang.top/gtbexdyzse.html

[R20] 关联数组（字典）
来源：http://hz.shuidangran.top/gtcoduwgmm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.ehwqpu.com/gtgjwjxbfq.html

[R21] 字符串长度
来源：http://hz.svipenyu.cn/gtlzjoamnk.html

echo "${#s}"
来源：http://hz.ppjwa.cn/gtypjprbvv.html

[R22] 截取子串
来源：http://hz.sxryk.cn/gtwnfkeluz.html

echo "${s:0:5}"
来源：http://hz.snrcjt.cn/gtpqxtywbg.html

[R23] 字符串替换
来源：http://hz.shangyingyoupin.top/gtwmalarja.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jyoumei.cn/gtfwmhaxqs.html

[R24] 大小写转换
来源：http://hz.hywenlv.cn/gttzjvtwai.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.gzhubu.top/gtomrxieal.html

[R25] 去后缀 / 去前缀
来源：http://hz.guowangkeji.top/gtubdamogd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.shanyushiyangtech.top/gtjtxselao.html

[R26] 命令替换
来源：http://hz.jinyuanbaomall.cn/gtxqobjrul.html

now=$(date +%F); echo "$now"
来源：http://hz.dianchejie.cn/gteftkvikt.html

[R27] 算术展开
来源：http://hz.52xcode.cn/gtxrjcjhdt.html

echo $((1 + 2 * 3))
来源：http://hz.316326.xyz/gttswwencb.html

[R28] 浮点运算
来源：http://hz.zhaomingkeji.xyz/gtjyfabtwn.html

echo "scale=2; 10/3" | bc
来源：http://hz.hnxiangtu.top/gtnndmedjv.html

[R29] 定义函数
来源：http://hz.aizwys.cn/gtuyolpada.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.smart0.xyz/gtkdszhgbf.html

[R30] 函数返回状态码
来源：http://hz.fengsongda.top/gtclrbpraj.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.snrcjt.cn/gtubomyolw.html

[R31] 局部变量
来源：http://hz.wangshuangyany.cn/gtjtuczztk.html

f() { local x=1; echo "$x"; }
来源：http://hz.sufxvd.cn/gtmhdmatug.html

[R32] 参数个数校验
来源：http://hz.cqqwz.cn/gtvoiojxda.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.tian-w.cn/gtomvdwcsz.html

[R33] 捕获错误并提示行号
来源：http://hz.chenlongwang.top/gtfktajzzs.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jiagoushi.top/gtewwoncpj.html

[R34] 退出时清理
来源：http://hz.cdnleiting.top/gthvsikyhf.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.9152youxi.cn/gtlbtoeovz.html

[R35] 后台执行并等待
来源：http://hz.zhixingplan.top/gttbjwuzct.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jyoumei.cn/gtzdetzsme.html

[R36] 并发执行多个任务
来源：http://hz.tanke756.top/gtiauuxcgp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.hfpthk.cn/gtecoudsqc.html

[R37] 把输出赋给变量
来源：http://hz.9152youxi.cn/gtxyqneucf.html

files=$(ls -1)
来源：http://hz.zhongyouzk.top/gtdqzvadxi.html

[R38] 管道串联
来源：http://hz.havefunace.top/gteclspxlg.html

cat a.txt | grep -i error | wc -l
来源：http://hz.meibo888.top/gtuywenave.html

[R39] 重定向标准输出与错误
来源：http://hz.hongshengwenyu.top/gtzvjdfsmr.html

cmd > out.log 2>&1
来源：http://hz.tianlin.xyz/gtxeezfisq.html

[R40] 追加写日志
来源：http://hz.cucudq.cn/gtaddadhdu.html

echo "log" >> out.log
来源：http://hz.chenlongwang.top/gttggsllwc.html

[R41] 丢弃输出
来源：http://hz.yanxiufei.cn/gtnketxduj.html

cmd >/dev/null 2>&1
来源：http://hz.zhaomingkeji.xyz/gtjpxwecmt.html

[R42] 输入重定向
来源：http://hz.ehwqpu.com/gtuztexfpn.html

wc -l < a.txt
来源：http://hz.fzhhl.top/gtzqbbewcn.html

[R43] 按名字查找文件
来源：http://hz.9152youxi.cn/gtuevbcvoy.html

find . -name "*.log" -type f
来源：http://hz.gotoacloud.top/gtktopxxne.html

[R44] 按修改时间查找
来源：http://hz.jlsjyb.cn/gtqrhzeabl.html

find . -mtime -7 -type f
来源：http://hz.havefunace.top/gtargnggva.html

[R45] 批量删除
来源：http://hz.ydzc1.top/gtrgnyklgs.html

find . -name "*.tmp" -delete
来源：http://hz.mhx1999.top/gthhlaueum.html

[R46] 递归替换文件内容
来源：http://hz.cqqwz.cn/gtliybfpio.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.9152youxi.cn/gtsbusqzhy.html

[R47] sed 单行替换
来源：http://hz.hnxiangtu.top/gtocqdjdtx.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.iojbl.cn/gtitkdjilk.html

[R48] awk 取指定列
来源：http://hz.jlsjyb.cn/gtxyuhxznb.html

awk '{print $1, $3}' a.txt
来源：http://hz.jyoumei.cn/gtkajbxhfo.html

[R49] awk 带条件
来源：http://hz.xuetiantiany.cn/gtvpoubppz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.nwbrower.top/gtjeqeudcj.html

[R50] awk 求和
来源：http://hz.daria6918.cn/gtjafvioqf.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.chenlongwang.top/gtknthknpk.html

[R51] 排序去重取前几
来源：http://hz.meibo888.top/gtgjhhkrli.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.dashuyun.cn/gtsxrhrafp.html

[R52] 统计行数
来源：http://hz.jqgufenzy.top/gtrcwuayya.html

wc -l a.txt
来源：http://hz.yuanzhike.top/gtnjbbbhcv.html

[R53] 查看文件头与实时尾
来源：http://hz.hammf.cn/gtzrxtaxec.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.316326.xyz/gtlxamthbi.html

[R54] 比较两个文件
来源：http://hz.quarkkingdee.top/gttdgpsrdm.html

diff a.txt b.txt
来源：http://hz.yuxming.cn/gtadvfnvck.html

[R55] 压缩与解压
来源：http://hz.hysaishi.cn/gtgnrsxszq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.cheryme.top/gtdvyscrcd.html

[R56] 远程拷贝
来源：http://hz.tian-w.cn/gtmrommsge.html

scp file user@host:/path/
来源：http://hz.yuanzhike.top/gthugummdf.html

[R57] 远程执行命令
来源：http://hz.gaohongyu789.top/gtgkdczjqp.html

ssh user@host 'uptime'
来源：http://hz.ppjwa.cn/gtrenzgftp.html

[R58] 下载文件
来源：http://hz.vqdsnc.cn/gtsmoiqinc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jlsjyb.cn/gtpyyjoukh.html

[R59] 发 POST JSON
来源：http://hz.yj202588.top/gtstnemjwl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.aibaodan.cn/gtktizeinq.html

[R60] 只看 HTTP 状态码
来源：http://hz.zhixingplan.top/gtglewgxcz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.vqdsnc.cn/gtxannmjdx.html

[R61] 磁盘占用
来源：http://hz.yanxiufei.cn/gtfmiiklrf.html

df -h;  du -sh *
来源：http://hz.zhaomingkeji.xyz/gtfotdcyzz.html

[R62] 找最占空间的文件
来源：http://hz.bjfxy.top/gtjsapsjcs.html

du -ah . | sort -rh | head -10
来源：http://hz.sufxvd.cn/gtplojzuhi.html

[R63] 内存与进程
来源：http://hz.xuanzx.com/gtedtvkoxy.html

free -h;  ps aux | grep nginx
来源：http://hz.vqdsnc.cn/gtqmfdhkzw.html

[R64] 结束进程
来源：http://hz.svipenyu.cn/gtkdbksdvy.html

kill -9 $(pgrep -f app.py)
来源：http://hz.xuetiantiany.cn/gtlvljihuz.html

[R65] 查看端口占用
来源：http://hz.tianlin.xyz/gtqmhtdrns.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.gogol.net.cn/gtdmfdmgsr.html

[R66] 定时任务
来源：http://hz.pengpengdd.cyou/gtguspyqgg.html

crontab -e;  crontab -l
来源：http://hz.birdmap.top/gtcvjnzqgg.html

[R67] 生成随机十六进制串
来源：http://hz.316326.xyz/gtakorahpl.html

openssl rand -hex 16
来源：http://hz.cucudq.cn/gtpdmmjgin.html

[R68] 计算文件校验值
来源：http://hz.jinqigfzy.top/gtyviggurd.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.shangyingyoupin.top/gtgeoroybe.html

[R69] 生成随机密码
来源：http://hz.sxryk.cn/gthueqaocw.html

head -c 16 /dev/urandom | base64
来源：http://hz.jlsjyb.cn/gtymcerlfy.html

[R70] 时间戳与互转
来源：http://hz.andypj.xyz/gtgdbdwqxk.html

date +%s;  date -d @1700000000
来源：http://hz.xuetiantiany.cn/gtbuntugvc.html

[R71] 日期格式化
来源：http://hz.shanyushiyangtech.top/gtpjucclct.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jiagoushi.top/gtwmmiyeqr.html

[R72] 等待端口就绪
来源：http://hz.hongshengwenyu.top/gtnaqvzlxm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.hywenlv.cn/gtjphznnyz.html

[R73] 分割大日志
来源：http://hz.daxiang520.top/gtgckyilpp.html

split -l 1000 big.log part_
来源：http://hz.fengsongda.top/gtpsnavsla.html

[R74] 批量重命名
来源：http://hz.jinqigfzy.top/gtayzzpads.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.316326.xyz/gtilbytdez.html

[R75] 导出环境变量
来源：http://hz.zhaomingkeji.xyz/gtnyixilnl.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.sxryk.cn/gtfpswqhil.html

[R76] 使用临时文件
来源：http://hz.daria6918.cn/gtkxpbdgiy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.hfpthk.cn/gtvuqsncmx.html

[R77] 读取用户输入
来源：http://hz.smart0.xyz/gtpfijzgzj.html

read -rp "请输入: " ans
来源：http://hz.kuanghao11.cn/gtwbnrdddq.html

[R78] 交互式菜单
来源：http://hz.zycfv.cn/gtciqiqgiw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.gzhubu.top/gtbonbvdjz.html

[R79] 解析命令行选项
来源：http://hz.xingfuxueyuan.xyz/gthmeiyqty.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.iojbl.cn/gttzsqmpnj.html

[R80] 查看脚本执行耗时
来源：http://hz.smart0.xyz/gtyujmcuxa.html

time ./run.sh
来源：http://hz.sweek.top/gtyxxjpidf.html

================================================================================
来源：http://hz.jyoumei.cn/gtacvgdwql.html

S. C / C++ 专题
来源：http://hz.xuetiantiany.cn/gthzqtcwne.html

================================================================================
来源：http://hz.tian-w.cn/gtaumczhbv.html

[S01] C：Hello World
来源：http://hz.zhiwuduotai.top/gtvsnhwuti.html

#include <stdio.h>
来源：http://hz.dianchejie.cn/gtyjtqezvj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.shzxlz.cn/gtnfbpxoaf.html

[S02] C：变量与格式化输出
来源：http://hz.zhaomingkeji.xyz/gtwvhumhcl.html

int a = 10; printf("%d\n", a);
来源：http://hz.shanyushiyangtech.top/gteokmggag.html

[S03] C：读入整数
来源：http://hz.jianghu66.top/gtyqfuplsj.html

int x; scanf("%d", &x);
来源：http://hz.yonumen.top/gtipmsgdsf.html

[S04] C：字符串复制
来源：http://hz.gzhubu.top/gtacpgiooo.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zhixingplan.top/gtehzzyfix.html

[S05] C：字符串长度
来源：http://hz.chenzaomai.com/gtanpholig.html

strlen(s)
来源：http://hz.yanxiufei.cn/gtqxneskkw.html

[S06] C：字符串比较
来源：http://hz.jqgufenzy.top/gtlxqsanxt.html

strcmp(a, b) == 0
来源：http://hz.xuetiantiany.cn/gtwjoaunxz.html

[S07] C：数组遍历求和
来源：http://hz.xylfe.cn/gtervjvvgp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.zycfv.cn/gthtxverar.html

[S08] C：动态内存分配与释放
来源：http://hz.xinyue.icu/gtnmacmris.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jqgufenzy.top/gtuhkjykxu.html

[S09] C：结构体定义与初始化
来源：http://hz.yj202588.top/gtlmnintes.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.tianlin.xyz/gtcearrrjc.html

[S10] C：指针与解引用
来源：http://hz.jinqigufen.top/gtpugwyrfo.html

int *p = &a;  *p = 5;
来源：http://hz.tianlin.xyz/gtfepepgwr.html

[S11] C：逐行读文件
来源：http://hz.9152youxi.cn/gtmawrthtc.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.pycfn.com/gtagfodjme.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.zhixingplan.top/gtjanspweb.html

fclose(f);
来源：http://hz.xingfuxueyuan.xyz/gtenpgasau.html

[S12] C：写文件
来源：http://hz.zdqjudy.top/gtmnwhwaun.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.c1oappe.top/gtubzydbyo.html

[S13] C：宏定义
来源：http://hz.jinqigufen.top/gtpnekljvq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.mhx1999.top/gtyiicmexq.html

[S14] C：枚举
来源：http://hz.ivvv.top/gthopvklix.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.shzxlz.cn/gtvsuosjuv.html

[S15] C：类型转换
来源：http://hz.aizwys.cn/gtdrkhfpfx.html

(double) a / b
来源：http://hz.shangyingyoupin.top/gtfcggughk.html

[S16] C：位操作置位
来源：http://hz.yanxiufei.cn/gtrlgqjwcr.html

x |= (1 << 3);
来源：http://hz.9152youxi.cn/gttsmepffq.html

[S17] C：安全拼接字符串
来源：http://hz.gaohongyu789.top/gtvwdqmtvs.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.yanxiufei.cn/gtkvzrgfjw.html

[S18] C：命令行参数
来源：http://hz.zdqjudy.top/gtuntauefm.html

int main(int argc, char **argv)
来源：http://hz.cashguo.top/gtnwzyhbic.html

[S19] C：快速排序
来源：http://hz.xinyue.icu/gthgxpuktz.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.hammf.cn/gtwmjcjxqb.html

[S20] C：二分查找
来源：http://hz.chenjidiqi.icu/gtapsrblee.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.mhx1999.top/gtztmeqjtv.html

[S21] C：字符类别判断
来源：http://hz.yj20258888.top/gtgubgenoh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jinyuanbaomall.cn/gtxkeyxdbz.html

[S22] C：字符串转数字
来源：http://hz.xuetiantiany.cn/gtdxbqeyru.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.daxiang520.top/gtodsirnoy.html

[S23] C：随机数
来源：http://hz.sxryk.cn/gtlwcdfekv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.0kj1m.cn/gthlgjslhy.html

[S24] C：获取本地时间
来源：http://hz.birdmap.top/gtepgyeapn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.hfpthk.cn/gtklfwtnuv.html

[S25] C：内存拷贝
来源：http://hz.haohaochexian.top/gtqasbyjlw.html

memcpy(dst, src, n);
来源：http://hz.zycfv.cn/gtezueinet.html

[S26] C：内存清零
来源：http://hz.xylfe.cn/gtypaveofx.html

memset(a, 0, sizeof a);
来源：http://hz.meibo888.top/gtcbrpkqkj.html

[S27] C：定义常量
来源：http://hz.iojbl.cn/gtibkqcmji.html

const double PI = 3.14159;
来源：http://hz.hongshengwenyu.top/gtgukrhodz.html

[S28] C：静态变量
来源：http://hz.jqgufenzy.top/gtovalwbnq.html

static int counter = 0;
来源：http://hz.pycfn.com/gtdlnjbunq.html

[S29] C：变参函数
来源：http://hz.sxryk.cn/gtedbyhmyx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.shuidangran.top/gtgitxeqhc.html

[S30] C：头文件保护
来源：http://hz.ybcxt.top/gtrqbwmuql.html

#ifndef X_H
来源：http://hz.yj202588.top/gtmgsfnats.html

#define X_H
来源：http://hz.xinyue.icu/gtsidfokyn.html

#endif
来源：http://hz.tianlin.xyz/gttumdxixm.html

[S31] C++：Hello World
来源：http://hz.havefunace.top/gtyfmxfaum.html

#include <iostream>
来源：http://hz.sufxvd.cn/gtgpmyxhgt.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.snrcjt.cn/gtlsjgblok.html

[S32] C++：字符串
来源：http://hz.xingfuxueyuan.xyz/gtkxwkveli.html

std::string s = "hi";  s += "!";
来源：http://hz.hfpthk.cn/gtdkglkqsm.html

[S33] C++：vector 增删
来源：http://hz.xuetiantiany.cn/gtdzphwpaz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.sxryk.cn/gtjoalmzid.html

[S34] C++：遍历 vector
来源：http://hz.cqqwz.cn/gtnukxfmhd.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.aibaodan.cn/gtearovncw.html

[S35] C++：map
来源：http://hz.0kj1m.cn/gtlgzloywb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hammf.cn/gtojzzfaxz.html

[S36] C++：unordered_map
来源：http://hz.hysaishi.cn/gtlqnfpqrg.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.sxryk.cn/gtozlmcuva.html

[S37] C++：set
来源：http://hz.nwbrower.top/gtjaohyvvt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.xingfuxueyuan.xyz/gtzrecooqh.html

[S38] C++：排序
来源：http://hz.yvedp.cn/gtntvhobtx.html

std::sort(v.begin(), v.end());
来源：http://hz.pycfn.com/gtgleuyvxw.html

[S39] C++：自定义比较器排序
来源：http://hz.nanxuanxn.top/gtmwumasto.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.nwbrower.top/gtocwrfmyv.html

[S40] C++：查找元素
来源：http://hz.nwbrower.top/gtxxsxvnvm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.cqqwz.cn/gtdnhikpny.html

[S41] C++：类与构造函数
来源：http://hz.gaohongyu789.top/gtueziyfzc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.snrcjt.cn/gtiluhpvis.html

[S42] C++：继承与虚函数
来源：http://hz.cdnleiting.top/gtvehjdcnm.html

class B : public Base { public: void f() override {} };
来源：http://hz.cashguo.top/gtqeoevlsz.html

[S43] C++：智能指针
来源：http://hz.tanke756.top/gtobfsiicq.html

auto p = std::make_unique<int>(5);
来源：http://hz.shanyushiyangtech.top/gtwnyijrhp.html

[S44] C++：引用传参
来源：http://hz.yj20258.top/gtriglwycc.html

void inc(int &x) { ++x; }
来源：http://hz.sweek.top/gtxcfpgkvk.html

[S45] C++：lambda
来源：http://hz.pengpengdd.cyou/gtcpvhwxaa.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.sysykeji.top/gtjkthbyov.html

[S46] C++：函数模板
来源：http://hz.ivvv.top/gtnryomkeg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.shanyushiyangkeji.top/gtqtuynecc.html

[S47] C++：结构化绑定遍历
来源：http://hz.xziqi.cn/gtiqrzduuy.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.hnxiangtu.top/gtiekxgxwv.html

[S48] C++：逐行读文件
来源：http://hz.ppjwa.cn/gtdqlspzta.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.andypj.xyz/gtoluitrrh.html

while (std::getline(in, line)) { }
来源：http://hz.guowangkeji.top/gtqrijkyzz.html

[S49] C++：写文件
来源：http://hz.jinqigfzy.top/gtssnsrzvv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.zhoulong.xyz/gtsslturws.html

[S50] C++：格式化数字
来源：http://hz.pengpengdd.cyou/gtfxuxkiwk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.nanxuanxn.top/gttzlijdlk.html

[S51] C++：显式类型转换
来源：http://hz.shzxlz.cn/gtficgwruw.html

static_cast<double>(a) / b
来源：http://hz.daxiang520.top/gtdtucvhra.html

[S52] C++：const 与 noexcept
来源：http://hz.guowangkeji.top/gtiwwpllkt.html

int size() const noexcept { return n_; }
来源：http://hz.yanxiufei.cn/gtohzkteag.html

[S53] C++：移动语义
来源：http://hz.tanke756.top/gtaoyhgogw.html

std::vector<int> w = std::move(v);
来源：http://hz.zhaomingkeji.xyz/gtzmxqflmj.html

[S54] C++：异常处理
来源：http://hz.hnqzz.top/gtzjgpqshd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.zdqjudy.top/gterqnupwu.html

[S55] C++：结构化绑定
来源：http://hz.xylfe.cn/gthhackatm.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.0kj1m.cn/gteajyropd.html

[S56] C++：optional
来源：http://hz.tianlin.xyz/gtofmnreve.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.shanyushiyangtech.top/gtmibxlfkt.html

[S57] C++：编译期常量
来源：http://hz.shuidangran.top/gtohkjwfvu.html

constexpr int N = 10;
来源：http://hz.xylfe.cn/gtxdcryqmj.html

[S58] C++：命名空间
来源：http://hz.havefunace.top/gtnmpbhham.html

namespace ns { int f() { return 1; } }
来源：http://hz.guowangkeji.top/gtheizqkfo.html

[S59] C++：静态断言
来源：http://hz.zhiwuduotai.top/gtcxnajssn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.aibaodan.cn/gtdfgcfmrp.html

[S60] C++：遍历并删除元素
来源：http://hz.shzxlz.cn/gtvqgqgeer.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.wangshuangyany.cn/gtqejkkfor.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtmcbozhjx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.hongshengwenyu.top/gtltcppdaw.html

================================================================================
来源：http://hz.xylfe.cn/gtcqjddaun.html

[T01] Kotlin：Hello World
来源：http://hz.yangfankeji.com/gtpdqzyhod.html

println("Hello")
来源：http://hz.wangshuangyany.cn/gtbycjhxvg.html

[T02] Kotlin：变量
来源：http://hz.cheryme.top/gtglotimvb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.tanke756.top/gtvnnjrqev.html

[T03] Kotlin：字符串模板
来源：http://hz.xingfuxueyuan.xyz/gtnikmbzmi.html

"值: $b"
来源：http://hz.zycfv.cn/gthfikisqo.html

[T04] Kotlin：空安全
来源：http://hz.shzxlz.cn/gtvzfzdwhv.html

val n: String? = null;  n?.length
来源：http://hz.zhaomingkeji.xyz/gtprtrzebm.html


<!-- 参考信息 -->