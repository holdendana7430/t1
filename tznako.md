代发 wailian999

name="${1:-default}"
来源：http://hz.shangyingyoupin.top/gtxilnavxk.html

[R06] 判断命令是否存在
来源：http://hz.cheryme.top/gtxihdjwlz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yvedp.cn/gtjrqtiagh.html

[R07] if 判断文件
来源：http://hz.yj20258888.top/gtmtjqyror.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.redwolf501.top/gtrchuhlyw.html

[R08] 数值比较
来源：http://hz.fzhhl.top/gtznkkoahn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.xziqi.cn/gtzfelviez.html

[R09] 字符串比较
来源：http://hz.tanke756.top/gtmzihlugg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.xuetiantiany.cn/gtspalfmro.html

[R10] 正则匹配
来源：http://hz.jqgufenzy.top/gtbinjyfdt.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yvedp.cn/gtkfgnwpoi.html

[R11] case 多分支
来源：http://hz.xinyue.icu/gteobejtbp.html

case "$1" in
来源：http://hz.gaohongyu789.top/gttwlgdgzm.html

start) echo "启动" ;;
来源：http://hz.shanyushiyangkeji.top/gtjhueopuh.html

stop)  echo "停止" ;;
来源：http://hz.nwbrower.top/gthogqncwv.html

*)     echo "未知命令" ;;
来源：http://hz.jinqigufen.top/gtfbclgjdb.html

esac
来源：http://hz.zhixingplan.top/gtvtrrftbq.html

[R12] for 遍历文件
来源：http://hz.jinghuilouyu.cn/gtllttsrjo.html

for f in *.txt; do echo "$f"; done
来源：http://hz.nanxuanxn.top/gtdqppdwcg.html

[R13] for 计数循环
来源：http://hz.jinqigufen.top/gtzllcaucj.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.meibo888.top/gtwfuxzzjn.html

[R14] C 风格 for
来源：http://hz.jqgfzy.top/gtubbcssfw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.pengpengdd.cyou/gtjnsavsci.html

[R15] while 逐行读文件
来源：http://hz.hongshengwenyu.top/gtnmpffhkl.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.gotoacloud.top/gtqqzyxpli.html

[R16] until 等待条件
来源：http://hz.sysykeji.top/gtojflasdx.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.havefunace.top/gtfuznggct.html

[R17] 数组定义与取值
来源：http://hz.jinghuilouyu.cn/gtangmrzzh.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yj20258888.top/gthuyvgvlx.html

[R18] 遍历数组
来源：http://hz.aibaodan.cn/gtljbeqixb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.yueranfly.top/gtnzwmtsyv.html

[R19] 数组长度
来源：http://hz.cdnleiting.top/gtqwyphrkj.html

echo "${#arr[@]}"
来源：http://hz.yongpay.top/gtnxakxxtd.html

[R20] 关联数组（字典）
来源：http://hz.hammf.cn/gtgbyujzdx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.vqdsnc.cn/gtusgiqogo.html

[R21] 字符串长度
来源：http://hz.jiagoushi.top/gtpsfozfvy.html

echo "${#s}"
来源：http://hz.0kj1m.cn/gtsyrurqma.html

[R22] 截取子串
来源：http://hz.c1oappe.top/gtyputiuqq.html

echo "${s:0:5}"
来源：http://hz.xylfe.cn/gtnbhptfvq.html

[R23] 字符串替换
来源：http://hz.jyoumei.cn/gtiseuljng.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.daxiang520.top/gtyhcizxtj.html

[R24] 大小写转换
来源：http://hz.9152youxi.cn/gtnjvbsgfg.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.jiagoushi.top/gtuggontwp.html

[R25] 去后缀 / 去前缀
来源：http://hz.wangshuangyany.cn/gtrwwvescn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.cheryme.top/gtyoccrikn.html

[R26] 命令替换
来源：http://hz.jinghuilouyu.cn/gthkvfokxh.html

now=$(date +%F); echo "$now"
来源：http://hz.bjfxy.top/gthtdvlcao.html

[R27] 算术展开
来源：http://hz.ywan-chungtsiang.top/gthbzdmquu.html

echo $((1 + 2 * 3))
来源：http://hz.aizwys.cn/gtsekilmha.html

[R28] 浮点运算
来源：http://hz.shanyushiyangtech.top/gtvvwkvpxw.html

echo "scale=2; 10/3" | bc
来源：http://hz.hysaishi.cn/gthkgywlvt.html

[R29] 定义函数
来源：http://hz.sufxvd.cn/gtqrewughp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.chenlongwang.top/gtjhdrmaum.html

[R30] 函数返回状态码
来源：http://hz.tianlin.xyz/gtbsfpfzrn.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.zhoulong.xyz/gtrjbxmfjt.html

[R31] 局部变量
来源：http://hz.snrcjt.cn/gtijsjciju.html

f() { local x=1; echo "$x"; }
来源：http://hz.dashuyun.cn/gtjksaohaa.html

[R32] 参数个数校验
来源：http://hz.jlsjyb.cn/gtwojkcsur.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.daxiang520.top/gtovyiknmw.html

[R33] 捕获错误并提示行号
来源：http://hz.sxryk.cn/gtrhbvpiuz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.0kj1m.cn/gtoicthryg.html

[R34] 退出时清理
来源：http://hz.havefunace.top/gtnkyiayvd.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.gaohongyu789.top/gtxkkatpdg.html

[R35] 后台执行并等待
来源：http://hz.chenzaomai.com/gtkempojor.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.shanyushiyangtech.top/gtyzkyoroo.html

[R36] 并发执行多个任务
来源：http://hz.tanke756.top/gthanjnavk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yonumen.top/gtsmdqhjyy.html

[R37] 把输出赋给变量
来源：http://hz.shanyushiyangkeji.top/gtjmqlgofc.html

files=$(ls -1)
来源：http://hz.aizwys.cn/gtpfqmovbv.html

[R38] 管道串联
来源：http://hz.birdmap.top/gtiuvfgxxx.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yvedp.cn/gtsxtmihlh.html

[R39] 重定向标准输出与错误
来源：http://hz.yonumen.top/gtyhleqjwd.html

cmd > out.log 2>&1
来源：http://hz.pengpengdd.cyou/gthcgvikbw.html

[R40] 追加写日志
来源：http://hz.sweek.top/gtdhpwtsbe.html

echo "log" >> out.log
来源：http://hz.ehwqpu.com/gttwrcppfk.html

[R41] 丢弃输出
来源：http://hz.chenlongwang.top/gthvjkpadr.html

cmd >/dev/null 2>&1
来源：http://hz.jianghu66.top/gtgyjwomvw.html

[R42] 输入重定向
来源：http://hz.sysykeji.top/gtmaffizyd.html

wc -l < a.txt
来源：http://hz.zhaomingkeji.xyz/gtfllrinaw.html

[R43] 按名字查找文件
来源：http://hz.havefunace.top/gtkfxbgwwy.html

find . -name "*.log" -type f
来源：http://hz.yongpay.top/gtmduobrvp.html

[R44] 按修改时间查找
来源：http://hz.yanxiufei.cn/gtvbnqiidf.html

find . -mtime -7 -type f
来源：http://hz.hnxiangtu.top/gtcazzavaj.html

[R45] 批量删除
来源：http://hz.jianghu66.top/gtfrkgraig.html

find . -name "*.tmp" -delete
来源：http://hz.sysykeji.top/gtxrldhrsb.html

[R46] 递归替换文件内容
来源：http://hz.sufxvd.cn/gtfaapvlyv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zhixingplan.top/gtyqbjuxak.html

[R47] sed 单行替换
来源：http://hz.tianlin.xyz/gtcybaalwx.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yuanzhike.top/gtojasbxtz.html

[R48] awk 取指定列
来源：http://hz.sysykeji.top/gtvtbtfcfu.html

awk '{print $1, $3}' a.txt
来源：http://hz.yj202588.top/gtkxomereb.html

[R49] awk 带条件
来源：http://hz.jinqigufen.top/gtrvqevkyz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.xingfuxueyuan.xyz/gtitunhmtl.html

[R50] awk 求和
来源：http://hz.gotoacloud.top/gtxuxeimyo.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.iojbl.cn/gtrmezaoca.html

[R51] 排序去重取前几
来源：http://hz.xylfe.cn/gtkbhtudbp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jinghuilouyu.cn/gtllmdtfds.html

[R52] 统计行数
来源：http://hz.jqgfzy.top/gtcikamgtp.html

wc -l a.txt
来源：http://hz.tianlin.xyz/gtiemigdxw.html

[R53] 查看文件头与实时尾
来源：http://hz.yj20258888.top/gtwmqkokbx.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.zhaomingkeji.xyz/gtchqyqltt.html

[R54] 比较两个文件
来源：http://hz.yj20258.top/gtotavngwg.html

diff a.txt b.txt
来源：http://hz.xingfuxueyuan.xyz/gtgpndsmkc.html

[R55] 压缩与解压
来源：http://hz.zhoulong.xyz/gtjynlcjql.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.shuidangran.top/gtsjbhommz.html

[R56] 远程拷贝
来源：http://hz.andypj.xyz/gtneqkvhho.html

scp file user@host:/path/
来源：http://hz.jqgufenzy.top/gtywcyjwxd.html

[R57] 远程执行命令
来源：http://hz.shzxlz.cn/gtpklwocfg.html

ssh user@host 'uptime'
来源：http://hz.sufxvd.cn/gtovynejkx.html

[R58] 下载文件
来源：http://hz.zhijiandao.cn/gtoqfrdpea.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.cqqwz.cn/gtqkesrqcv.html

[R59] 发 POST JSON
来源：http://hz.chenzaomai.com/gthdyjctie.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yueranfly.top/gtzkifhdug.html

[R60] 只看 HTTP 状态码
来源：http://hz.cashguo.top/gteciakuvc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.yuxming.cn/gtoybopgpc.html

[R61] 磁盘占用
来源：http://hz.zhaomingkeji.xyz/gtkapoqaor.html

df -h;  du -sh *
来源：http://hz.ppjwa.cn/gtgovdwtgo.html

[R62] 找最占空间的文件
来源：http://hz.aizwys.cn/gtvfnfdnal.html

du -ah . | sort -rh | head -10
来源：http://hz.hywenlv.cn/gtfxwkzush.html

[R63] 内存与进程
来源：http://hz.tian-w.cn/gtrsplelds.html

free -h;  ps aux | grep nginx
来源：http://hz.ywan-chungtsiang.top/gtyibzkmzz.html

[R64] 结束进程
来源：http://hz.zhixingplan.top/gtrdkpdtpg.html

kill -9 $(pgrep -f app.py)
来源：http://hz.ehwqpu.com/gthkbawtul.html

[R65] 查看端口占用
来源：http://hz.xuanzx.com/gtpzpnufra.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.guowangkeji.top/gtsktokcdr.html

[R66] 定时任务
来源：http://hz.cucudq.cn/gtfpijjucu.html

crontab -e;  crontab -l
来源：http://hz.yj202588.top/gtnxhwcgrs.html

[R67] 生成随机十六进制串
来源：http://hz.fzhhl.top/gtpuatvnoc.html

openssl rand -hex 16
来源：http://hz.jqgufenzy.top/gtygesfpgo.html

[R68] 计算文件校验值
来源：http://hz.zhengqikj.top/gttyejoprh.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yuxming.cn/gtshmpmwcv.html

[R69] 生成随机密码
来源：http://hz.vqdsnc.cn/gtfweoezoj.html

head -c 16 /dev/urandom | base64
来源：http://hz.ydzc1.top/gtmnenloem.html

[R70] 时间戳与互转
来源：http://hz.haohaochexian.top/gtcmdojxxa.html

date +%s;  date -d @1700000000
来源：http://hz.jqgufenzy.top/gtvrlryips.html

[R71] 日期格式化
来源：http://hz.gaohongyu789.top/gthymdxfao.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jlsjyb.cn/gtbkrqhefj.html

[R72] 等待端口就绪
来源：http://hz.redwolf501.top/gtbgqyprrf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.sufxvd.cn/gtfpwuzywp.html

[R73] 分割大日志
来源：http://hz.hysaishi.cn/gteyulglha.html

split -l 1000 big.log part_
来源：http://hz.wangshuangyany.cn/gtnuhatrfa.html

[R74] 批量重命名
来源：http://hz.daria6918.cn/gtvyrpsxbh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.pengpengdd.cyou/gtivydzzkd.html

[R75] 导出环境变量
来源：http://hz.cdnleiting.top/gtrtfkaoyu.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.zhijiandao.cn/gtpzzjzjxh.html

[R76] 使用临时文件
来源：http://hz.kuanghao11.cn/gtkbsmaytl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.nwbrower.top/gttlgrwqjv.html

[R77] 读取用户输入
来源：http://hz.bjfxy.top/gtgmqltjnm.html

read -rp "请输入: " ans
来源：http://hz.cucudq.cn/gtvqhqinhl.html

[R78] 交互式菜单
来源：http://hz.pycfn.com/gtesdlogiv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.daria6918.cn/gtagjzdloz.html

[R79] 解析命令行选项
来源：http://hz.nwbrower.top/gtzjgrjefy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.shanyushiyangkeji.top/gtuagibdgv.html

[R80] 查看脚本执行耗时
来源：http://hz.havefunace.top/gtknlkacfx.html

time ./run.sh
来源：http://hz.zhaomingkeji.xyz/gtbzafludw.html

================================================================================
来源：http://hz.jianghu66.top/gtapxqbjvk.html

S. C / C++ 专题
来源：http://hz.aibaodan.cn/gtjndlpgkc.html

================================================================================
来源：http://hz.yongpay.top/gtgaiylrei.html

[S01] C：Hello World
来源：http://hz.yangfankeji.com/gtnbnujcuo.html

#include <stdio.h>
来源：http://hz.52xcode.cn/gtrkufbamh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.aizwys.cn/gtzxmbndil.html

[S02] C：变量与格式化输出
来源：http://hz.bjfxy.top/gthynrljwf.html

int a = 10; printf("%d\n", a);
来源：http://hz.cdnleiting.top/gtrfxskenh.html

[S03] C：读入整数
来源：http://hz.hysaishi.cn/gtnlwsqbhb.html

int x; scanf("%d", &x);
来源：http://hz.jlsjyb.cn/gtmgmgfxyr.html

[S04] C：字符串复制
来源：http://hz.guannengcc.top/gtvxcpzlpb.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.nanxinkj.top/gtrrufpgla.html

[S05] C：字符串长度
来源：http://hz.xinyue.icu/gtqpfbasqe.html

strlen(s)
来源：http://hz.pengpengdd.cyou/gtzfaoazrj.html

[S06] C：字符串比较
来源：http://hz.dianchejie.cn/gtoqusurab.html

strcmp(a, b) == 0
来源：http://hz.fzhhl.top/gtbgwwajbc.html

[S07] C：数组遍历求和
来源：http://hz.vqdsnc.cn/gtlunahhdo.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.sufxvd.cn/gtvbiehore.html

[S08] C：动态内存分配与释放
来源：http://hz.redwolf501.top/gtprstrnnh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yvedp.cn/gtgxyluafi.html

[S09] C：结构体定义与初始化
来源：http://hz.ybcxt.top/gtjcskzbaq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.feifeiyinyue.top/gtwhrailfm.html

[S10] C：指针与解引用
来源：http://hz.xylfe.cn/gtuxrxcfks.html

int *p = &a;  *p = 5;
来源：http://hz.zhixingplan.top/gtqjhhmbej.html

[S11] C：逐行读文件
来源：http://hz.havefunace.top/gtcznsmalv.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.hammf.cn/gtbfoejuwl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.gogol.net.cn/gthopndrcg.html

fclose(f);
来源：http://hz.hnqzz.top/gttwdvanwu.html

[S12] C：写文件
来源：http://hz.meibo888.top/gtezaxhbsv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.nwbrower.top/gtxfefgehq.html

[S13] C：宏定义
来源：http://hz.jinghuilouyu.cn/gtbamnmvvv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.zhongyouzk.top/gtfmgtgpqd.html

[S14] C：枚举
来源：http://hz.ppjwa.cn/gtbmlvmfmm.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.xziqi.cn/gtqdjalyaa.html

[S15] C：类型转换
来源：http://hz.52xcode.cn/gtfilfwmqg.html

(double) a / b
来源：http://hz.birdmap.top/gtxmzkfnqf.html

[S16] C：位操作置位
来源：http://hz.shuidangran.top/gtwmqzkcyi.html

x |= (1 << 3);
来源：http://hz.yuxming.cn/gtyzeczeys.html

[S17] C：安全拼接字符串
来源：http://hz.zhiwuduotai.top/gtgqhjfqjw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.zhijiandao.cn/gturybwpfd.html

[S18] C：命令行参数
来源：http://hz.sweek.top/gtremygqwa.html

int main(int argc, char **argv)
来源：http://hz.guowangkeji.top/gtytkowmef.html

[S19] C：快速排序
来源：http://hz.yuanzhike.top/gtvogoqklu.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.mhx1999.top/gtmaggholq.html

[S20] C：二分查找
来源：http://hz.yj20258888.top/gtlijvppui.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yanxiufei.cn/gtvosqcwex.html

[S21] C：字符类别判断
来源：http://hz.yj202588.top/gtizbsfsya.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.shuidangran.top/gtiwjszbqy.html

[S22] C：字符串转数字
来源：http://hz.chenlongwang.top/gtlnckxpgy.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yueranfly.top/gtzxldmqhr.html

[S23] C：随机数
来源：http://hz.daxiang520.top/gtyptyhdhb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.shzxlz.cn/gtsrgobndr.html

[S24] C：获取本地时间
来源：http://hz.yj20258888.top/gtrdwibppi.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.xingfuxueyuan.xyz/gtksewdycx.html

[S25] C：内存拷贝
来源：http://hz.yj202588.top/gtuduxamia.html

memcpy(dst, src, n);
来源：http://hz.316326.xyz/gtbcjpklnv.html

[S26] C：内存清零
来源：http://hz.hfpthk.cn/gtcnbybxhr.html

memset(a, 0, sizeof a);
来源：http://hz.shangyingyoupin.top/gtjwmifgsp.html

[S27] C：定义常量
来源：http://hz.smart0.xyz/gtnjegrcwt.html

const double PI = 3.14159;
来源：http://hz.gotoacloud.top/gtrmypvzix.html

[S28] C：静态变量
来源：http://hz.xuetiantiany.cn/gthyammunz.html

static int counter = 0;
来源：http://hz.tian-w.cn/gtdxmwoaxa.html

[S29] C：变参函数
来源：http://hz.aibaodan.cn/gtiwbfxgxk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.0kj1m.cn/gtvolmqyln.html

[S30] C：头文件保护
来源：http://hz.ydjk.org.cn/gtkgunrpcs.html

#ifndef X_H
来源：http://hz.zhixingplan.top/gtbuywzsfh.html

#define X_H
来源：http://hz.tian-w.cn/gtbwhdsjry.html

#endif
来源：http://hz.quarkkingdee.top/gtitetgfli.html

[S31] C++：Hello World
来源：http://hz.sxryk.cn/gtugiqjjfa.html

#include <iostream>
来源：http://hz.yongpay.top/gtpmngykiv.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.zhengqikj.top/gtakwcffhr.html

[S32] C++：字符串
来源：http://hz.yuanzhike.top/gtguvqlazr.html

std::string s = "hi";  s += "!";
来源：http://hz.gaohongyu789.top/gttkioqtau.html

[S33] C++：vector 增删
来源：http://hz.wangshuangyany.cn/gtutqiofim.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.shanyushiyangkeji.top/gthbidwcgz.html

[S34] C++：遍历 vector
来源：http://hz.hnqzz.top/gtcrytsylg.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.shanyushiyangtech.top/gthtzepfzw.html

[S35] C++：map
来源：http://hz.quarkkingdee.top/gtbzakiyhj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jiagoushi.top/gtswvaigjd.html

[S36] C++：unordered_map
来源：http://hz.birdmap.top/gtcqhgklhj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jqgufenzy.top/gtdgmitqpi.html

[S37] C++：set
来源：http://hz.yuanzhike.top/gtlrqdagth.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.0kj1m.cn/gtwmnofods.html

[S38] C++：排序
来源：http://hz.ywan-chungtsiang.top/gtnylsydqo.html

std::sort(v.begin(), v.end());
来源：http://hz.sweek.top/gtbjyvuigj.html

[S39] C++：自定义比较器排序
来源：http://hz.nanxinkj.top/gtfnqzkwbs.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.iojbl.cn/gtdyryxtyn.html

[S40] C++：查找元素
来源：http://hz.sufxvd.cn/gtwqyhdour.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.tian-w.cn/gtmdbbppst.html

[S41] C++：类与构造函数
来源：http://hz.chenzaomai.com/gtjgqdbuad.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.dashuyun.cn/gtnkjipclt.html

[S42] C++：继承与虚函数
来源：http://hz.zycfv.cn/gtfnsnogcn.html

class B : public Base { public: void f() override {} };
来源：http://hz.zhengqikj.top/gtwhgjciwd.html

[S43] C++：智能指针
来源：http://hz.fzhhl.top/gtvqpehgog.html

auto p = std::make_unique<int>(5);
来源：http://hz.gaohongyu789.top/gtfeyirlur.html

[S44] C++：引用传参
来源：http://hz.shangyingyoupin.top/gtgxzvccjf.html

void inc(int &x) { ++x; }
来源：http://hz.yonumen.top/gtinxcprrv.html

[S45] C++：lambda
来源：http://hz.jinyuanbaomall.cn/gtygpazwmd.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.xingfuxueyuan.xyz/gtrikiqrfn.html

[S46] C++：函数模板
来源：http://hz.dashuyun.cn/gtnedftcfm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yuxming.cn/gtmzztobln.html

[S47] C++：结构化绑定遍历
来源：http://hz.zhoulong.xyz/gtilbymais.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.hywenlv.cn/gtxkansugi.html

[S48] C++：逐行读文件
来源：http://hz.pycfn.com/gtkomjkpyb.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.xylfe.cn/gtacsjuvma.html

while (std::getline(in, line)) { }
来源：http://hz.shangyingyoupin.top/gtahcevqim.html

[S49] C++：写文件
来源：http://hz.yanxiufei.cn/gtaiejfllh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.daxiang520.top/gtxzrgetfn.html

[S50] C++：格式化数字
来源：http://hz.smart0.xyz/gtinpxzoyw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.nanxuanxn.top/gtydilhbnc.html

[S51] C++：显式类型转换
来源：http://hz.yvedp.cn/gtteefcumb.html

static_cast<double>(a) / b
来源：http://hz.jqgfzy.top/gteygcuvxt.html

[S52] C++：const 与 noexcept
来源：http://hz.jinghuilouyu.cn/gtskdivsyr.html

int size() const noexcept { return n_; }
来源：http://hz.daxiang520.top/gtiyltnsfg.html

[S53] C++：移动语义
来源：http://hz.chenzaomai.com/gtxyxiohgp.html

std::vector<int> w = std::move(v);
来源：http://hz.316326.xyz/gtidlqquuq.html

[S54] C++：异常处理
来源：http://hz.sxryk.cn/gtjgfbzqfr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.jyoumei.cn/gtzoqdizlk.html

[S55] C++：结构化绑定
来源：http://hz.hammf.cn/gtwgjpdrch.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.shangyingyoupin.top/gtzbttkutt.html

[S56] C++：optional
来源：http://hz.wangdashe.top/gtulyubnbf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.zdqjudy.top/gtmeqbgujn.html

[S57] C++：编译期常量
来源：http://hz.snrcjt.cn/gtyyfrkuwd.html

constexpr int N = 10;
来源：http://hz.316326.xyz/gtlietfnoc.html

[S58] C++：命名空间
来源：http://hz.mhx1999.top/gtsmnavcue.html

namespace ns { int f() { return 1; } }
来源：http://hz.cdnleiting.top/gtpvxtiupl.html

[S59] C++：静态断言
来源：http://hz.shuidangran.top/gtgybmmhia.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.yvedp.cn/gtmcqjmmib.html

[S60] C++：遍历并删除元素
来源：http://hz.52xcode.cn/gtszjdkndv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yonumen.top/gttbfufpnw.html

================================================================================
来源：http://hz.nwbrower.top/gtccfhksmg.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zycfv.cn/gtyylebmnp.html

================================================================================
来源：http://hz.kuanghao11.cn/gtfpxqzqeg.html

[T01] Kotlin：Hello World
来源：http://hz.zhijiandao.cn/gtoeyuxsyw.html

println("Hello")
来源：http://hz.meibo888.top/gtajspcbxb.html

[T02] Kotlin：变量
来源：http://hz.zhongyouzk.top/gtxiprwvsc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.haohaochexian.top/gtahixbwck.html

[T03] Kotlin：字符串模板
来源：http://hz.hammf.cn/gtagmxzakx.html

"值: $b"
来源：http://hz.yuanzhike.top/gtpkmfcekm.html

[T04] Kotlin：空安全
来源：http://hz.cucudq.cn/gtnuckmszd.html

val n: String? = null;  n?.length
来源：http://hz.yanxiufei.cn/gtoalbqvfm.html

[T05] Kotlin：when 表达式
来源：http://hz.quarkkingdee.top/gttxxlzkqe.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.ybcxt.top/gtacxzajyr.html

[T06] Kotlin：集合映射
来源：http://hz.cucudq.cn/gtrfglowrj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.0kj1m.cn/gtvhyqozqw.html


<!-- 参考信息 -->