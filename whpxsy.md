代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.tian-w.cn/gtzgkqhyaf.html

[R08] 数值比较
来源：http://hz.zhengqikj.top/gtkzoiljqp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.cucudq.cn/gtfkzncdkb.html

[R09] 字符串比较
来源：http://hz.guowangkeji.top/gtuuvapdca.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.sysykeji.top/gtziwdmnbv.html

[R10] 正则匹配
来源：http://hz.hnxiangtu.top/gtofwkpddp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.meibo888.top/gtfzjntdgn.html

[R11] case 多分支
来源：http://hz.fzhhl.top/gtpodfduhi.html

case "$1" in
来源：http://hz.guowangkeji.top/gtmpgknckr.html

start) echo "启动" ;;
来源：http://hz.gotoacloud.top/gthzjuzarr.html

stop)  echo "停止" ;;
来源：http://hz.wangdashe.top/gtzrweossa.html

*)     echo "未知命令" ;;
来源：http://hz.iojbl.cn/gtxnkqtozr.html

esac
来源：http://hz.jinqigufen.top/gtpcnwhbzl.html

[R12] for 遍历文件
来源：http://hz.svipenyu.cn/gtwbxaguds.html

for f in *.txt; do echo "$f"; done
来源：http://hz.ehwqpu.com/gthlvkzltf.html

[R13] for 计数循环
来源：http://hz.yangfankeji.com/gtfvuohsyr.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.xylfe.cn/gthrtdvdej.html

[R14] C 风格 for
来源：http://hz.ppjwa.cn/gtaxmfuhqi.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.52xcode.cn/gthnfhguiz.html

[R15] while 逐行读文件
来源：http://hz.yonumen.top/gthafocsua.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jyoumei.cn/gtupkfqoth.html

[R16] until 等待条件
来源：http://hz.yj20258888.top/gtwdthvkrc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.tanke756.top/gtvvdcpwdb.html

[R17] 数组定义与取值
来源：http://hz.shzxlz.cn/gtnwmlxnnx.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jlsjyb.cn/gthufvuood.html

[R18] 遍历数组
来源：http://hz.ybcxt.top/gtengrqejq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.sxryk.cn/gtcragokwb.html

[R19] 数组长度
来源：http://hz.hywenlv.cn/gtnznujvvz.html

echo "${#arr[@]}"
来源：http://hz.hfpthk.cn/gtcgbeogpq.html

[R20] 关联数组（字典）
来源：http://hz.chenjidiqi.icu/gtwubmmdom.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.cucudq.cn/gtadiaoybt.html

[R21] 字符串长度
来源：http://hz.cashguo.top/gtqwxqdqom.html

echo "${#s}"
来源：http://hz.xziqi.cn/gtcvhopzmc.html

[R22] 截取子串
来源：http://hz.cqqwz.cn/gtopuyhytg.html

echo "${s:0:5}"
来源：http://hz.sysykeji.top/gtfzdeomli.html

[R23] 字符串替换
来源：http://hz.feifeiyinyue.top/gtwiklqflx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.yj20258888.top/gtgjyviwcl.html

[R24] 大小写转换
来源：http://hz.yj202588.top/gtlinudsvd.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.shanyushiyangkeji.top/gtvdvslurk.html

[R25] 去后缀 / 去前缀
来源：http://hz.ywan-chungtsiang.top/gtfjtttvdy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.gaohongyu789.top/gtxtkkhlsy.html

[R26] 命令替换
来源：http://hz.aizwys.cn/gturbivtlj.html

now=$(date +%F); echo "$now"
来源：http://hz.kuanghao11.cn/gtspgmbpms.html

[R27] 算术展开
来源：http://hz.jinqigfzy.top/gtkiuefxxz.html

echo $((1 + 2 * 3))
来源：http://hz.hammf.cn/gtoidnvlfb.html

[R28] 浮点运算
来源：http://hz.jinyuanbaomall.cn/gtshzeaizo.html

echo "scale=2; 10/3" | bc
来源：http://hz.xingfuxueyuan.xyz/gtqqeuvkza.html

[R29] 定义函数
来源：http://hz.ybcxt.top/gtanqkixcl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.cucudq.cn/gtgoezrvid.html

[R30] 函数返回状态码
来源：http://hz.nanxuanxn.top/gtwoggwcod.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.feifeiyinyue.top/gtrzbfhzcx.html

[R31] 局部变量
来源：http://hz.shanyushiyangkeji.top/gtyainsfdw.html

f() { local x=1; echo "$x"; }
来源：http://hz.jinqigfzy.top/gtinugmbhv.html

[R32] 参数个数校验
来源：http://hz.shanyushiyangkeji.top/gtxdznykdy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.xingfuxueyuan.xyz/gtzabugeji.html

[R33] 捕获错误并提示行号
来源：http://hz.gogol.net.cn/gtlneyqaiw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.tanke756.top/gtszcjhsfj.html

[R34] 退出时清理
来源：http://hz.jinqigfzy.top/gtjqzjmcjk.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.ywan-chungtsiang.top/gthlogfjjz.html

[R35] 后台执行并等待
来源：http://hz.fzhhl.top/gtcyekssae.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.cheryme.top/gtypdgaeru.html

[R36] 并发执行多个任务
来源：http://hz.zhoulong.xyz/gtbaixxzbx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jinqigfzy.top/gtbaidiraj.html

[R37] 把输出赋给变量
来源：http://hz.yj20258.top/gtekhwhyxf.html

files=$(ls -1)
来源：http://hz.ywan-chungtsiang.top/gtdtgexgbf.html

[R38] 管道串联
来源：http://hz.tian-w.cn/gtjbyvcicm.html

cat a.txt | grep -i error | wc -l
来源：http://hz.xuanzx.com/gttzzjhenj.html

[R39] 重定向标准输出与错误
来源：http://hz.gzhubu.top/gthyqdqzxk.html

cmd > out.log 2>&1
来源：http://hz.chenzaomai.com/gtodmblvgx.html

[R40] 追加写日志
来源：http://hz.zhongyouzk.top/gtqpjjziqt.html

echo "log" >> out.log
来源：http://hz.yueranfly.top/gtugxenbgn.html

[R41] 丢弃输出
来源：http://hz.yonumen.top/gthmaavjbs.html

cmd >/dev/null 2>&1
来源：http://hz.gotoacloud.top/gtexoqvfnm.html

[R42] 输入重定向
来源：http://hz.yangfankeji.com/gtpdzzzmvu.html

wc -l < a.txt
来源：http://hz.xuetiantiany.cn/gtkunwduhw.html

[R43] 按名字查找文件
来源：http://hz.xuanzx.com/gtvfwepzod.html

find . -name "*.log" -type f
来源：http://hz.andypj.xyz/gttpwccbls.html

[R44] 按修改时间查找
来源：http://hz.haohaochexian.top/gtbvpccacb.html

find . -mtime -7 -type f
来源：http://hz.zhongyouzk.top/gtokncfphj.html

[R45] 批量删除
来源：http://hz.shuidangran.top/gtfotusiog.html

find . -name "*.tmp" -delete
来源：http://hz.cashguo.top/gtjplgrpni.html

[R46] 递归替换文件内容
来源：http://hz.cucudq.cn/gtxmfpuyme.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.hnqzz.top/gtvofirevn.html

[R47] sed 单行替换
来源：http://hz.iojbl.cn/gtotdllrpu.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.mhx1999.top/gtxebjynme.html

[R48] awk 取指定列
来源：http://hz.yueranfly.top/gtgmjjpdtp.html

awk '{print $1, $3}' a.txt
来源：http://hz.redwolf501.top/gtbtmyyxtt.html

[R49] awk 带条件
来源：http://hz.yvedp.cn/gtykgqokpz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.dianchejie.cn/gtjrxskvot.html

[R50] awk 求和
来源：http://hz.tian-w.cn/gtiigbqocw.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.zhaomingkeji.xyz/gtgcxtmkdl.html

[R51] 排序去重取前几
来源：http://hz.snrcjt.cn/gtkryqulcd.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.zhongyouzk.top/gtmthmjvcs.html

[R52] 统计行数
来源：http://hz.shzxlz.cn/gtdnozsuic.html

wc -l a.txt
来源：http://hz.gaohongyu789.top/gtkvxqmtcs.html

[R53] 查看文件头与实时尾
来源：http://hz.shanyushiyangkeji.top/gttjisqwan.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.dianchejie.cn/gtwfbnuwmk.html

[R54] 比较两个文件
来源：http://hz.jinqigufen.top/gtaddfwhjm.html

diff a.txt b.txt
来源：http://hz.jinghuilouyu.cn/gthtsohghs.html

[R55] 压缩与解压
来源：http://hz.jyoumei.cn/gtoparnlot.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.smart0.xyz/gtryuphnrv.html

[R56] 远程拷贝
来源：http://hz.daria6918.cn/gttknbkjut.html

scp file user@host:/path/
来源：http://hz.andypj.xyz/gtlnzsnmhe.html

[R57] 远程执行命令
来源：http://hz.hongshengwenyu.top/gtdalycain.html

ssh user@host 'uptime'
来源：http://hz.aibaodan.cn/gtdtwpgoxc.html

[R58] 下载文件
来源：http://hz.guowangkeji.top/gtqjrtifcf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.nanxinkj.top/gtuulowllt.html

[R59] 发 POST JSON
来源：http://hz.mhx1999.top/gtdknhusil.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jinqigfzy.top/gtjkrhyfuj.html

[R60] 只看 HTTP 状态码
来源：http://hz.9152youxi.cn/gtuvvpwqik.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.316326.xyz/gtsmlgiiwl.html

[R61] 磁盘占用
来源：http://hz.yongpay.top/gtugraebut.html

df -h;  du -sh *
来源：http://hz.jqgfzy.top/gthsxbuihf.html

[R62] 找最占空间的文件
来源：http://hz.hongshengwenyu.top/gtkynbcuoa.html

du -ah . | sort -rh | head -10
来源：http://hz.yanxiufei.cn/gtbcramjdo.html

[R63] 内存与进程
来源：http://hz.shanyushiyangkeji.top/gtnbobgvyy.html

free -h;  ps aux | grep nginx
来源：http://hz.jinyuanbaomall.cn/gtpyrhjbmj.html

[R64] 结束进程
来源：http://hz.chenlongwang.top/gthqlqyngj.html

kill -9 $(pgrep -f app.py)
来源：http://hz.quarkkingdee.top/gtztvwxiuw.html

[R65] 查看端口占用
来源：http://hz.jiagoushi.top/gtyomkdbmf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.hywenlv.cn/gtubdbchtk.html

[R66] 定时任务
来源：http://hz.guannengcc.top/gtjbragpwq.html

crontab -e;  crontab -l
来源：http://hz.hammf.cn/gtlgaghpnk.html

[R67] 生成随机十六进制串
来源：http://hz.ppjwa.cn/gtbzydykfq.html

openssl rand -hex 16
来源：http://hz.svipenyu.cn/gtzwcssrrg.html

[R68] 计算文件校验值
来源：http://hz.ydjk.org.cn/gtndajxwrf.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.shangyingyoupin.top/gtrzwjmxtm.html

[R69] 生成随机密码
来源：http://hz.jiagoushi.top/gtgnkuwnek.html

head -c 16 /dev/urandom | base64
来源：http://hz.hysaishi.cn/gttlptzyif.html

[R70] 时间戳与互转
来源：http://hz.zycfv.cn/gtdhitbsdi.html

date +%s;  date -d @1700000000
来源：http://hz.nwbrower.top/gtoggsbhyl.html

[R71] 日期格式化
来源：http://hz.chenzaomai.com/gtoddxqgxk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.xuetiantiany.cn/gtlhbksvyz.html

[R72] 等待端口就绪
来源：http://hz.316326.xyz/gtjcciurvi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jinyuanbaomall.cn/gtyxchgpso.html

[R73] 分割大日志
来源：http://hz.yonumen.top/gteaabueba.html

split -l 1000 big.log part_
来源：http://hz.jinqigufen.top/gtftctcsex.html

[R74] 批量重命名
来源：http://hz.hongshengwenyu.top/gtfbvczixq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.gzhubu.top/gtpwqgkgva.html

[R75] 导出环境变量
来源：http://hz.9152youxi.cn/gtdumgxqhc.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.c1oappe.top/gtvmuubkad.html

[R76] 使用临时文件
来源：http://hz.0kj1m.cn/gtcpniwmmo.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.hnxiangtu.top/gtrucciuhb.html

[R77] 读取用户输入
来源：http://hz.sysykeji.top/gtpugthmtg.html

read -rp "请输入: " ans
来源：http://hz.ehwqpu.com/gtxixkpmgn.html

[R78] 交互式菜单
来源：http://hz.yanxiufei.cn/gtnqmfpley.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.haohaochexian.top/gtktlshyut.html

[R79] 解析命令行选项
来源：http://hz.jinghuilouyu.cn/gtqmokknxd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.hammf.cn/gtugyjygvn.html

[R80] 查看脚本执行耗时
来源：http://hz.tian-w.cn/gthaseefnd.html

time ./run.sh
来源：http://hz.nwbrower.top/gtxtsmmfhp.html

================================================================================
来源：http://hz.sxryk.cn/gtqlkhszyz.html

S. C / C++ 专题
来源：http://hz.yonumen.top/gthipwaylf.html

================================================================================
来源：http://hz.gogol.net.cn/gteccvmefl.html

[S01] C：Hello World
来源：http://hz.tianlin.xyz/gtuxrptidx.html

#include <stdio.h>
来源：http://hz.quarkkingdee.top/gtkueengim.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.zdqjudy.top/gtwkmezwly.html

[S02] C：变量与格式化输出
来源：http://hz.zhijiandao.cn/gtuwdrezlq.html

int a = 10; printf("%d\n", a);
来源：http://hz.nwbrower.top/gtxnkykskq.html

[S03] C：读入整数
来源：http://hz.meibo888.top/gtgjszlycu.html

int x; scanf("%d", &x);
来源：http://hz.guannengcc.top/gtopfajfgm.html

[S04] C：字符串复制
来源：http://hz.zdqjudy.top/gtyvlsprag.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.ydzc1.top/gthcfszika.html

[S05] C：字符串长度
来源：http://hz.nanxuanxn.top/gtugcjplmh.html

strlen(s)
来源：http://hz.yuanzhike.top/gtcvbhnkvd.html

[S06] C：字符串比较
来源：http://hz.gotoacloud.top/gtehxbpabt.html

strcmp(a, b) == 0
来源：http://hz.cheryme.top/gtrayfelta.html

[S07] C：数组遍历求和
来源：http://hz.shangyingyoupin.top/gtflrgqgss.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.snrcjt.cn/gtgbkbbodd.html

[S08] C：动态内存分配与释放
来源：http://hz.yangfankeji.com/gtkxwaoscv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.shanyushiyangkeji.top/gtxjvwgxzb.html

[S09] C：结构体定义与初始化
来源：http://hz.chenzaomai.com/gtkommwbaa.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yonumen.top/gtdhtkkcci.html

[S10] C：指针与解引用
来源：http://hz.jqgufenzy.top/gtciartxyu.html

int *p = &a;  *p = 5;
来源：http://hz.yonumen.top/gtdxxjsejm.html

[S11] C：逐行读文件
来源：http://hz.yangfankeji.com/gtfrklzdjj.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.zhiwuduotai.top/gtclduxfgb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.ydjk.org.cn/gtdclnzudf.html

fclose(f);
来源：http://hz.zhongyouzk.top/gtdacubedd.html

[S12] C：写文件
来源：http://hz.jinghuilouyu.cn/gtxiuhbjjp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.ybcxt.top/gteakchhra.html

[S13] C：宏定义
来源：http://hz.fengsongda.top/gtnaloazgl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.zhoulong.xyz/gtbquknewc.html

[S14] C：枚举
来源：http://hz.jlsjyb.cn/gtaiwbqkfe.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.iojbl.cn/gtxgnfumrs.html

[S15] C：类型转换
来源：http://hz.cucudq.cn/gtovhwhuax.html

(double) a / b
来源：http://hz.wangshuangyany.cn/gtxiaemtxi.html

[S16] C：位操作置位
来源：http://hz.zhoulong.xyz/gtwycsrrwo.html

x |= (1 << 3);
来源：http://hz.shzxlz.cn/gtkgvikral.html

[S17] C：安全拼接字符串
来源：http://hz.yongpay.top/gtampmvswj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.shanyushiyangkeji.top/gtatxrpwha.html

[S18] C：命令行参数
来源：http://hz.wangshuangyany.cn/gtdwccvalj.html

int main(int argc, char **argv)
来源：http://hz.gotoacloud.top/gtkteixhnd.html

[S19] C：快速排序
来源：http://hz.smart0.xyz/gtbgcwnozy.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.gogol.net.cn/gtspgsccry.html

[S20] C：二分查找
来源：http://hz.ywan-chungtsiang.top/gtbrfeviph.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yongpay.top/gtqtanmfkd.html

[S21] C：字符类别判断
来源：http://hz.fengsongda.top/gtfesfhqzt.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.wangdashe.top/gtwrvzepkx.html

[S22] C：字符串转数字
来源：http://hz.kuanghao11.cn/gttutduwiw.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.sxryk.cn/gtsuhcnlpg.html

[S23] C：随机数
来源：http://hz.mhx1999.top/gtgpiviioa.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.andypj.xyz/gtmimssltf.html

[S24] C：获取本地时间
来源：http://hz.yj20258.top/gtrxcaruey.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.wangdashe.top/gtcxmzhykw.html

[S25] C：内存拷贝
来源：http://hz.zhiwuduotai.top/gtnpjrgzrz.html

memcpy(dst, src, n);
来源：http://hz.chenzaomai.com/gtcnxpnarh.html

[S26] C：内存清零
来源：http://hz.hysaishi.cn/gtqpfkkcoc.html

memset(a, 0, sizeof a);
来源：http://hz.shuidangran.top/gtxrmjpqhl.html

[S27] C：定义常量
来源：http://hz.sysykeji.top/gtsnajpjji.html

const double PI = 3.14159;
来源：http://hz.andypj.xyz/gtwbdeqvyp.html

[S28] C：静态变量
来源：http://hz.birdmap.top/gtzokqcjkf.html

static int counter = 0;
来源：http://hz.fzhhl.top/gtalxjwpkd.html

[S29] C：变参函数
来源：http://hz.havefunace.top/gtbthuqcup.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.daria6918.cn/gtelgemwpr.html

[S30] C：头文件保护
来源：http://hz.sxryk.cn/gtaunnpxtj.html

#ifndef X_H
来源：http://hz.52xcode.cn/gtvrbvkaly.html

#define X_H
来源：http://hz.ywan-chungtsiang.top/gtzllvujon.html

#endif
来源：http://hz.smart0.xyz/gtokutgvjj.html

[S31] C++：Hello World
来源：http://hz.cashguo.top/gtfyohtbsk.html

#include <iostream>
来源：http://hz.ydjk.org.cn/gtduiuofvb.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.c1oappe.top/gtftkdwtxz.html

[S32] C++：字符串
来源：http://hz.kuanghao11.cn/gtodxijafg.html

std::string s = "hi";  s += "!";
来源：http://hz.zycfv.cn/gtuwahtbxr.html

[S33] C++：vector 增删
来源：http://hz.gzhubu.top/gtxmmxdocq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yuxming.cn/gtbhdnxahx.html

[S34] C++：遍历 vector
来源：http://hz.yanxiufei.cn/gtbmzwmabx.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.chenjidiqi.icu/gtepfzskmk.html

[S35] C++：map
来源：http://hz.gogol.net.cn/gtfaivmage.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hammf.cn/gtjbpuhrdv.html

[S36] C++：unordered_map
来源：http://hz.hywenlv.cn/gtfsqottch.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ydjk.org.cn/gtdoiqxpjn.html

[S37] C++：set
来源：http://hz.cheryme.top/gtfprurola.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.zhijiandao.cn/gtwfduryrp.html

[S38] C++：排序
来源：http://hz.shuidangran.top/gtntceprjf.html

std::sort(v.begin(), v.end());
来源：http://hz.gzhubu.top/gtjrhmxwqp.html

[S39] C++：自定义比较器排序
来源：http://hz.316326.xyz/gtnaxfakwp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.wangdashe.top/gtuxdhapev.html

[S40] C++：查找元素
来源：http://hz.jinqigfzy.top/gtfdgcfnxg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.cashguo.top/gtrlhufzds.html

[S41] C++：类与构造函数
来源：http://hz.chenzaomai.com/gtrcqxocmo.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.svipenyu.cn/gtoqjnpejg.html

[S42] C++：继承与虚函数
来源：http://hz.chenjidiqi.icu/gtkmwnahxp.html

class B : public Base { public: void f() override {} };
来源：http://hz.zhengqikj.top/gttiwgbhxd.html

[S43] C++：智能指针
来源：http://hz.yanxiufei.cn/gtglovgbbc.html

auto p = std::make_unique<int>(5);
来源：http://hz.ydzc1.top/gtmvlnebhi.html

[S44] C++：引用传参
来源：http://hz.nanxuanxn.top/gtydeltxpv.html

void inc(int &x) { ++x; }
来源：http://hz.xuetiantiany.cn/gtdjtsdxks.html

[S45] C++：lambda
来源：http://hz.52xcode.cn/gtoqioucrq.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.shangyingyoupin.top/gtfrlowdsv.html

[S46] C++：函数模板
来源：http://hz.chenlongwang.top/gtunafolxm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zhoulong.xyz/gtnpvrtoyq.html

[S47] C++：结构化绑定遍历
来源：http://hz.aizwys.cn/gthgtkzvbw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.yanxiufei.cn/gtomlaolym.html

[S48] C++：逐行读文件
来源：http://hz.fzhhl.top/gtqnckzxxf.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.andypj.xyz/gtpspadsyk.html

while (std::getline(in, line)) { }
来源：http://hz.daria6918.cn/gtkvpntufd.html

[S49] C++：写文件
来源：http://hz.zhijiandao.cn/gtpxjdbiia.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.zhixingplan.top/gtrqukxshf.html

[S50] C++：格式化数字
来源：http://hz.xuanzx.com/gtoflpnnhl.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.birdmap.top/gtcimkayzd.html

[S51] C++：显式类型转换
来源：http://hz.cucudq.cn/gtnfjjrnpb.html

static_cast<double>(a) / b
来源：http://hz.zdqjudy.top/gtdxhduslo.html

[S52] C++：const 与 noexcept
来源：http://hz.shanyushiyangtech.top/gtdrqpgeyw.html

int size() const noexcept { return n_; }
来源：http://hz.yuanzhike.top/gtxplxtfml.html

[S53] C++：移动语义
来源：http://hz.wangshuangyany.cn/gtnbvvwhot.html

std::vector<int> w = std::move(v);
来源：http://hz.shzxlz.cn/gttbkmapkz.html

[S54] C++：异常处理
来源：http://hz.nwbrower.top/gtdrlcxveb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.ywan-chungtsiang.top/gtaqtedegs.html

[S55] C++：结构化绑定
来源：http://hz.svipenyu.cn/gtpyuebkah.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.quarkkingdee.top/gtudthrwlg.html

[S56] C++：optional
来源：http://hz.zhiwuduotai.top/gtqoejxvbi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.nanxinkj.top/gtqqlwixab.html

[S57] C++：编译期常量
来源：http://hz.cdnleiting.top/gtvvmvagla.html

constexpr int N = 10;
来源：http://hz.yueranfly.top/gtdcsrkwhw.html

[S58] C++：命名空间
来源：http://hz.chenjidiqi.icu/gtzjtrqxjm.html

namespace ns { int f() { return 1; } }
来源：http://hz.shanyushiyangkeji.top/gtaltkkpmf.html

[S59] C++：静态断言
来源：http://hz.aibaodan.cn/gtznimvjcs.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.xingfuxueyuan.xyz/gttlyktclm.html

[S60] C++：遍历并删除元素
来源：http://hz.meibo888.top/gtgzeswkes.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.quarkkingdee.top/gtvhcngiyt.html

================================================================================
来源：http://hz.mhx1999.top/gtjlphmdxo.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.ehwqpu.com/gtltuturcx.html

================================================================================
来源：http://hz.nanxinkj.top/gtmgxahhjg.html

[T01] Kotlin：Hello World
来源：http://hz.zhijiandao.cn/gtufevvkfd.html

println("Hello")
来源：http://hz.yvedp.cn/gtrhinqadm.html

[T02] Kotlin：变量
来源：http://hz.sufxvd.cn/gtghkvuqpt.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yangfankeji.com/gtcptbtfhp.html

[T03] Kotlin：字符串模板
来源：http://hz.jianghu66.top/gtjyhclisf.html

"值: $b"
来源：http://hz.52xcode.cn/gtrkafjhvm.html

[T04] Kotlin：空安全
来源：http://hz.zhixingplan.top/gtukajlqmj.html

val n: String? = null;  n?.length
来源：http://hz.zhiwuduotai.top/gtcxhyxnms.html

[T05] Kotlin：when 表达式
来源：http://hz.haohaochexian.top/gtszeulbbe.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.daxiang520.top/gtbekhkvlj.html

[T06] Kotlin：集合映射
来源：http://hz.chenzaomai.com/gtenuaczxp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jinyuanbaomall.cn/gtqdemdyrh.html

[T07] Kotlin：集合过滤
来源：http://hz.ehwqpu.com/gtjifuahey.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.havefunace.top/gteesairfa.html

[T08] Kotlin：数据类
来源：http://hz.hnqzz.top/gtyukznuym.html

data class User(val name: String, val age: Int)
来源：http://hz.yuxming.cn/gtqzbcpzub.html


<!-- 参考信息 -->