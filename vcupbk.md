代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.316326.xyz/gtahhkccxj.html

[R08] 数值比较
来源：http://hz.yonumen.top/gtxhtzcxql.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yj20258888.top/gtpjbxfxgx.html

[R09] 字符串比较
来源：http://hz.yueranfly.top/gtrnaupevy.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zhijiandao.cn/gtfukajlbu.html

[R10] 正则匹配
来源：http://hz.ehwqpu.com/gtkpclqcsx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.aibaodan.cn/gtzfteijrf.html

[R11] case 多分支
来源：http://hz.dashuyun.cn/gtkefasmqf.html

case "$1" in
来源：http://hz.svipenyu.cn/gtuzrdzeuf.html

start) echo "启动" ;;
来源：http://hz.wangdashe.top/gtwutoszjz.html

stop)  echo "停止" ;;
来源：http://hz.daria6918.cn/gtjezepadf.html

*)     echo "未知命令" ;;
来源：http://hz.guannengcc.top/gtdpbefloq.html

esac
来源：http://hz.shuidangran.top/gtiacoqbka.html

[R12] for 遍历文件
来源：http://hz.hammf.cn/gtpkkdzqwg.html

for f in *.txt; do echo "$f"; done
来源：http://hz.aibaodan.cn/gthikyprlh.html

[R13] for 计数循环
来源：http://hz.jqgfzy.top/gtkvlyeqzw.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jianghu66.top/gthdnwyehz.html

[R14] C 风格 for
来源：http://hz.zhiwuduotai.top/gtlnlhavwy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.nwbrower.top/gtszzdyyxj.html

[R15] while 逐行读文件
来源：http://hz.hnxiangtu.top/gtfuismvxx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.smart0.xyz/gtrrfagcnu.html

[R16] until 等待条件
来源：http://hz.hywenlv.cn/gtprhfeuit.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.zdqjudy.top/gtdfvazwcv.html

[R17] 数组定义与取值
来源：http://hz.0kj1m.cn/gtdavzrfox.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jinqigfzy.top/gtmyezhqei.html

[R18] 遍历数组
来源：http://hz.bjfxy.top/gtvkkbfdxm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.316326.xyz/gtcmrahife.html

[R19] 数组长度
来源：http://hz.ydjk.org.cn/gtqftudszi.html

echo "${#arr[@]}"
来源：http://hz.ydzc1.top/gtahjmiuif.html

[R20] 关联数组（字典）
来源：http://hz.cashguo.top/gtzvosevfs.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yonumen.top/gtgtzergsc.html

[R21] 字符串长度
来源：http://hz.yanxiufei.cn/gtkhtktyyi.html

echo "${#s}"
来源：http://hz.jinqigufen.top/gtrqpruiel.html

[R22] 截取子串
来源：http://hz.tianlin.xyz/gtsdbasevv.html

echo "${s:0:5}"
来源：http://hz.guowangkeji.top/gtozczkhfr.html

[R23] 字符串替换
来源：http://hz.sufxvd.cn/gthzbsbgde.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.daria6918.cn/gtstiptway.html

[R24] 大小写转换
来源：http://hz.zycfv.cn/gthjoxkivp.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.gotoacloud.top/gtuuseufap.html

[R25] 去后缀 / 去前缀
来源：http://hz.guannengcc.top/gtfpannrkq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.redwolf501.top/gtrjxttfrv.html

[R26] 命令替换
来源：http://hz.andypj.xyz/gtyquxnofs.html

now=$(date +%F); echo "$now"
来源：http://hz.quarkkingdee.top/gtoklxdrsb.html

[R27] 算术展开
来源：http://hz.nanxinkj.top/gtjkioihiq.html

echo $((1 + 2 * 3))
来源：http://hz.yj20258.top/gtdgsxghbt.html

[R28] 浮点运算
来源：http://hz.dianchejie.cn/gtjbqjdfeo.html

echo "scale=2; 10/3" | bc
来源：http://hz.chenzaomai.com/gtzwkwffzj.html

[R29] 定义函数
来源：http://hz.wangshuangyany.cn/gtbuxivzdd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.tian-w.cn/gtzaybzvlb.html

[R30] 函数返回状态码
来源：http://hz.tanke756.top/gtlkksicqp.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.gotoacloud.top/gtssbqmyva.html

[R31] 局部变量
来源：http://hz.iojbl.cn/gtrqjpgxuq.html

f() { local x=1; echo "$x"; }
来源：http://hz.yj20258.top/gtgyzvembd.html

[R32] 参数个数校验
来源：http://hz.nanxuanxn.top/gtbcnmmsqf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.zhixingplan.top/gtfgdhcoxp.html

[R33] 捕获错误并提示行号
来源：http://hz.dianchejie.cn/gtodcdogkx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.ppjwa.cn/gtvhxvljgr.html

[R34] 退出时清理
来源：http://hz.tanke756.top/gtpwlmodem.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.hysaishi.cn/gtntkdqsxj.html

[R35] 后台执行并等待
来源：http://hz.nwbrower.top/gtwrnwlmjg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.dianchejie.cn/gtwcphrvch.html

[R36] 并发执行多个任务
来源：http://hz.vqdsnc.cn/gtwvcmuasy.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.zhongyouzk.top/gtxmesjstl.html

[R37] 把输出赋给变量
来源：http://hz.nwbrower.top/gtntnaugkr.html

files=$(ls -1)
来源：http://hz.cheryme.top/gtetfwctkw.html

[R38] 管道串联
来源：http://hz.hfpthk.cn/gtqqehnnhs.html

cat a.txt | grep -i error | wc -l
来源：http://hz.ydzc1.top/gtxcbscyhk.html

[R39] 重定向标准输出与错误
来源：http://hz.jinqigfzy.top/gteewpltqy.html

cmd > out.log 2>&1
来源：http://hz.hywenlv.cn/gthnkjjnsu.html

[R40] 追加写日志
来源：http://hz.hammf.cn/gtidoehfhn.html

echo "log" >> out.log
来源：http://hz.ivvv.top/gtyfleongb.html

[R41] 丢弃输出
来源：http://hz.yongpay.top/gtjteozxei.html

cmd >/dev/null 2>&1
来源：http://hz.ybcxt.top/gtrqwfaksq.html

[R42] 输入重定向
来源：http://hz.ivvv.top/gtkwltjqhw.html

wc -l < a.txt
来源：http://hz.bjfxy.top/gthdrgotyl.html

[R43] 按名字查找文件
来源：http://hz.yvedp.cn/gtifrikhev.html

find . -name "*.log" -type f
来源：http://hz.ydjk.org.cn/gtjiipvmgq.html

[R44] 按修改时间查找
来源：http://hz.zhijiandao.cn/gtbutrappc.html

find . -mtime -7 -type f
来源：http://hz.gogol.net.cn/gtnmebmolx.html

[R45] 批量删除
来源：http://hz.zhengqikj.top/gtvgcrywoh.html

find . -name "*.tmp" -delete
来源：http://hz.guowangkeji.top/gtymbpfuuz.html

[R46] 递归替换文件内容
来源：http://hz.ivvv.top/gtrstztxvy.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.andypj.xyz/gtokihfgpw.html

[R47] sed 单行替换
来源：http://hz.c1oappe.top/gtlgahvlgu.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.nanxinkj.top/gtdeqwxrgl.html

[R48] awk 取指定列
来源：http://hz.zdqjudy.top/gtolrghdem.html

awk '{print $1, $3}' a.txt
来源：http://hz.pengpengdd.cyou/gtvhmclwnc.html

[R49] awk 带条件
来源：http://hz.c1oappe.top/gtofzldbct.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.xuetiantiany.cn/gtyihichkg.html

[R50] awk 求和
来源：http://hz.sxryk.cn/gtdklyihya.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.shzxlz.cn/gtdiqmwltm.html

[R51] 排序去重取前几
来源：http://hz.snrcjt.cn/gtrogwbxlu.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.shanyushiyangtech.top/gtpjgnkjah.html

[R52] 统计行数
来源：http://hz.yj20258888.top/gtbapzqyik.html

wc -l a.txt
来源：http://hz.9152youxi.cn/gtgzslqvpi.html

[R53] 查看文件头与实时尾
来源：http://hz.sxryk.cn/gtpmbupfit.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yj202588.top/gtwxgwfwfh.html

[R54] 比较两个文件
来源：http://hz.shanyushiyangkeji.top/gtxeexdhmw.html

diff a.txt b.txt
来源：http://hz.cdnleiting.top/gtdgowacbs.html

[R55] 压缩与解压
来源：http://hz.meibo888.top/gtlqtxnlzu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.cucudq.cn/gtakjkqprs.html

[R56] 远程拷贝
来源：http://hz.cdnleiting.top/gtdgaguflw.html

scp file user@host:/path/
来源：http://hz.snrcjt.cn/gtcvnjwzyc.html

[R57] 远程执行命令
来源：http://hz.guowangkeji.top/gtdcpzzufz.html

ssh user@host 'uptime'
来源：http://hz.zhaomingkeji.xyz/gtdnxqumro.html

[R58] 下载文件
来源：http://hz.gogol.net.cn/gtahzeceaa.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.cashguo.top/gtdbfazleb.html

[R59] 发 POST JSON
来源：http://hz.ehwqpu.com/gtlxhgemwi.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.gogol.net.cn/gtfejbxxla.html

[R60] 只看 HTTP 状态码
来源：http://hz.52xcode.cn/gtesdkyzuz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.hongshengwenyu.top/gtkpgdholj.html

[R61] 磁盘占用
来源：http://hz.yj20258888.top/gtnaoppofy.html

df -h;  du -sh *
来源：http://hz.cdnleiting.top/gtkynpprxp.html

[R62] 找最占空间的文件
来源：http://hz.cqqwz.cn/gtugrombvu.html

du -ah . | sort -rh | head -10
来源：http://hz.cdnleiting.top/gtglfauata.html

[R63] 内存与进程
来源：http://hz.tian-w.cn/gtvqnpyclp.html

free -h;  ps aux | grep nginx
来源：http://hz.zhongyouzk.top/gtyiikwtee.html

[R64] 结束进程
来源：http://hz.cqqwz.cn/gthvdiorqm.html

kill -9 $(pgrep -f app.py)
来源：http://hz.smart0.xyz/gtvccgpxug.html

[R65] 查看端口占用
来源：http://hz.xuetiantiany.cn/gthrdipwsl.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yongpay.top/gtbmadzqyw.html

[R66] 定时任务
来源：http://hz.quarkkingdee.top/gtsvtanrgl.html

crontab -e;  crontab -l
来源：http://hz.redwolf501.top/gtzhnhrgjo.html

[R67] 生成随机十六进制串
来源：http://hz.0kj1m.cn/gtzblzypnj.html

openssl rand -hex 16
来源：http://hz.ehwqpu.com/gtknwljivr.html

[R68] 计算文件校验值
来源：http://hz.andypj.xyz/gtewangzmf.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.pycfn.com/gtbdoblntr.html

[R69] 生成随机密码
来源：http://hz.snrcjt.cn/gtebylthpq.html

head -c 16 /dev/urandom | base64
来源：http://hz.guannengcc.top/gtyydzvubr.html

[R70] 时间戳与互转
来源：http://hz.kuanghao11.cn/gtwrehocek.html

date +%s;  date -d @1700000000
来源：http://hz.ehwqpu.com/gtbbuemahj.html

[R71] 日期格式化
来源：http://hz.c1oappe.top/gtoyfvygac.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.feifeiyinyue.top/gtnphbyxwa.html

[R72] 等待端口就绪
来源：http://hz.hysaishi.cn/gtdkkwnqee.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.aizwys.cn/gtdqdesqdw.html

[R73] 分割大日志
来源：http://hz.hysaishi.cn/gteuidifkn.html

split -l 1000 big.log part_
来源：http://hz.yuxming.cn/gtxuxnexgk.html

[R74] 批量重命名
来源：http://hz.ehwqpu.com/gtvpixefic.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jinyuanbaomall.cn/gtvnmfftml.html

[R75] 导出环境变量
来源：http://hz.chenjidiqi.icu/gtcdykwvtv.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.jlsjyb.cn/gtrrebqugy.html

[R76] 使用临时文件
来源：http://hz.gzhubu.top/gtjhrhpuuh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.cashguo.top/gtseetdnqs.html

[R77] 读取用户输入
来源：http://hz.zhijiandao.cn/gtfzoeipyq.html

read -rp "请输入: " ans
来源：http://hz.yj20258888.top/gthimdrcxm.html

[R78] 交互式菜单
来源：http://hz.ywan-chungtsiang.top/gtjwiwsedp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.daria6918.cn/gtvffhgexl.html

[R79] 解析命令行选项
来源：http://hz.xuetiantiany.cn/gtbcwzbgyv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.vqdsnc.cn/gtqrxyqbsa.html

[R80] 查看脚本执行耗时
来源：http://hz.yj202588.top/gtpacjsdgm.html

time ./run.sh
来源：http://hz.havefunace.top/gtvjdrujoe.html

================================================================================
来源：http://hz.hysaishi.cn/gtmeaiipel.html

S. C / C++ 专题
来源：http://hz.shuidangran.top/gtterphiey.html

================================================================================
来源：http://hz.xylfe.cn/gtfzxknwwb.html

[S01] C：Hello World
来源：http://hz.jyoumei.cn/gtfpttymwm.html

#include <stdio.h>
来源：http://hz.smart0.xyz/gttuatqxtm.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.gzhubu.top/gttegfimdd.html

[S02] C：变量与格式化输出
来源：http://hz.redwolf501.top/gtkisjczej.html

int a = 10; printf("%d\n", a);
来源：http://hz.yj20258888.top/gtmcrsysrs.html

[S03] C：读入整数
来源：http://hz.aizwys.cn/gtoaassryl.html

int x; scanf("%d", &x);
来源：http://hz.havefunace.top/gtnnalvind.html

[S04] C：字符串复制
来源：http://hz.dashuyun.cn/gtpzhbqewd.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.yvedp.cn/gtmnifpvgf.html

[S05] C：字符串长度
来源：http://hz.andypj.xyz/gtulzfckml.html

strlen(s)
来源：http://hz.jinyuanbaomall.cn/gttjeyiujl.html

[S06] C：字符串比较
来源：http://hz.hnxiangtu.top/gtwgtxqxkv.html

strcmp(a, b) == 0
来源：http://hz.hnxiangtu.top/gtannksogl.html

[S07] C：数组遍历求和
来源：http://hz.xuetiantiany.cn/gtrdunexsj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.gzhubu.top/gtbraiyeml.html

[S08] C：动态内存分配与释放
来源：http://hz.xuetiantiany.cn/gtojnopzmr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.ydzc1.top/gthpwosxbh.html

[S09] C：结构体定义与初始化
来源：http://hz.ydjk.org.cn/gtfzuwkmcn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yonumen.top/gttauyvffy.html

[S10] C：指针与解引用
来源：http://hz.redwolf501.top/gtlasrpkog.html

int *p = &a;  *p = 5;
来源：http://hz.jqgfzy.top/gtzshuoilv.html

[S11] C：逐行读文件
来源：http://hz.xinyue.icu/gtefrwgsaa.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.9152youxi.cn/gtvixnpgru.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.zhongyouzk.top/gtcbaeewuq.html

fclose(f);
来源：http://hz.jiagoushi.top/gteglgvijn.html

[S12] C：写文件
来源：http://hz.snrcjt.cn/gtchxzhopw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.guannengcc.top/gtkdkpiwxh.html

[S13] C：宏定义
来源：http://hz.birdmap.top/gtxitgzxkr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.chenzaomai.com/gtfavuhixd.html

[S14] C：枚举
来源：http://hz.ydzc1.top/gttcvmiouj.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.hywenlv.cn/gtspnwyuyd.html

[S15] C：类型转换
来源：http://hz.hnxiangtu.top/gticwwibuz.html

(double) a / b
来源：http://hz.jianghu66.top/gtxilqleva.html

[S16] C：位操作置位
来源：http://hz.ehwqpu.com/gtfgrfjmsb.html

x |= (1 << 3);
来源：http://hz.nanxinkj.top/gtdtduefif.html

[S17] C：安全拼接字符串
来源：http://hz.hongshengwenyu.top/gtagesjmzd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.zhoulong.xyz/gtggykvqup.html

[S18] C：命令行参数
来源：http://hz.hywenlv.cn/gtsinfunpf.html

int main(int argc, char **argv)
来源：http://hz.cdnleiting.top/gtphqhiyas.html

[S19] C：快速排序
来源：http://hz.nwbrower.top/gtiwvugrgf.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.zycfv.cn/gtzwvdolln.html

[S20] C：二分查找
来源：http://hz.ybcxt.top/gtsrzkcmwu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.cucudq.cn/gtzbnkvatt.html

[S21] C：字符类别判断
来源：http://hz.aizwys.cn/gtuuspglac.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.guannengcc.top/gtvjoslaeq.html

[S22] C：字符串转数字
来源：http://hz.zdqjudy.top/gtfwkvcfug.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.mhx1999.top/gtckgwbfkm.html

[S23] C：随机数
来源：http://hz.sysykeji.top/gthaqxublw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.pengpengdd.cyou/gtppqocmoe.html

[S24] C：获取本地时间
来源：http://hz.cdnleiting.top/gtcaflvxui.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.ivvv.top/gttgdprliz.html

[S25] C：内存拷贝
来源：http://hz.hnqzz.top/gtqojojkwa.html

memcpy(dst, src, n);
来源：http://hz.cashguo.top/gtifiqmclm.html

[S26] C：内存清零
来源：http://hz.tianlin.xyz/gtjsgtwnfa.html

memset(a, 0, sizeof a);
来源：http://hz.gaohongyu789.top/gtvmarbvtd.html

[S27] C：定义常量
来源：http://hz.c1oappe.top/gtltyvzfyk.html

const double PI = 3.14159;
来源：http://hz.zhongyouzk.top/gtwnqxmycu.html

[S28] C：静态变量
来源：http://hz.jqgufenzy.top/gtxemlcken.html

static int counter = 0;
来源：http://hz.aizwys.cn/gtmqbqrhgl.html

[S29] C：变参函数
来源：http://hz.cqqwz.cn/gthzuasmfu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.0kj1m.cn/gtsyzjoivm.html

[S30] C：头文件保护
来源：http://hz.xuanzx.com/gtoqzpvhzw.html

#ifndef X_H
来源：http://hz.haohaochexian.top/gtpqipfwct.html

#define X_H
来源：http://hz.sxryk.cn/gtihftffnp.html

#endif
来源：http://hz.gaohongyu789.top/gtibgivtgw.html

[S31] C++：Hello World
来源：http://hz.chenlongwang.top/gtwrjaetyt.html

#include <iostream>
来源：http://hz.jinqigufen.top/gtpkrannso.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.nanxinkj.top/gtdphffyub.html

[S32] C++：字符串
来源：http://hz.kuanghao11.cn/gtmzeanfhz.html

std::string s = "hi";  s += "!";
来源：http://hz.daria6918.cn/gtilitbwlh.html

[S33] C++：vector 增删
来源：http://hz.jianghu66.top/gtkjlzcdpz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.sufxvd.cn/gtbcvvnrur.html

[S34] C++：遍历 vector
来源：http://hz.zhijiandao.cn/gtxuimhlyn.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.cheryme.top/gtsygxmjmj.html

[S35] C++：map
来源：http://hz.hfpthk.cn/gtoarxnpzb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.bjfxy.top/gtlnekaxvp.html

[S36] C++：unordered_map
来源：http://hz.birdmap.top/gtawbbgawf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.fzhhl.top/gtmvxsgrbe.html

[S37] C++：set
来源：http://hz.pengpengdd.cyou/gtyfckjftd.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.52xcode.cn/gtewewjidi.html

[S38] C++：排序
来源：http://hz.tianlin.xyz/gttfuiqctx.html

std::sort(v.begin(), v.end());
来源：http://hz.wangdashe.top/gtnwjndpwk.html

[S39] C++：自定义比较器排序
来源：http://hz.yangfankeji.com/gtucgelubs.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.nanxinkj.top/gteputjqfn.html

[S40] C++：查找元素
来源：http://hz.pycfn.com/gtpgojtjno.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.xinyue.icu/gtpfyodsen.html

[S41] C++：类与构造函数
来源：http://hz.wangshuangyany.cn/gtkmfubycw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.9152youxi.cn/gtkmlyvyjy.html

[S42] C++：继承与虚函数
来源：http://hz.ppjwa.cn/gtflnchtlw.html

class B : public Base { public: void f() override {} };
来源：http://hz.havefunace.top/gtfdkjoirp.html

[S43] C++：智能指针
来源：http://hz.chenjidiqi.icu/gtgrrbtjgc.html

auto p = std::make_unique<int>(5);
来源：http://hz.zhongyouzk.top/gtkatnjkxv.html

[S44] C++：引用传参
来源：http://hz.jinyuanbaomall.cn/gtdvtlpjla.html

void inc(int &x) { ++x; }
来源：http://hz.tian-w.cn/gtgksmoowg.html

[S45] C++：lambda
来源：http://hz.dashuyun.cn/gtifcvotor.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.kuanghao11.cn/gtzjxpvgoa.html

[S46] C++：函数模板
来源：http://hz.ivvv.top/gttsfezxcl.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zhixingplan.top/gtjgjphlhf.html

[S47] C++：结构化绑定遍历
来源：http://hz.yuxming.cn/gtdgcmpyxm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.gzhubu.top/gtjwyvwypz.html

[S48] C++：逐行读文件
来源：http://hz.yj20258.top/gtbdbxtivn.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.sxryk.cn/gtzzsozraf.html

while (std::getline(in, line)) { }
来源：http://hz.sufxvd.cn/gtpvprowtj.html

[S49] C++：写文件
来源：http://hz.ppjwa.cn/gtieiihqir.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.daxiang520.top/gtujfqykqd.html

[S50] C++：格式化数字
来源：http://hz.quarkkingdee.top/gtrylsqadr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.nwbrower.top/gtotdzeeoh.html

[S51] C++：显式类型转换
来源：http://hz.guannengcc.top/gtityrgwxv.html

static_cast<double>(a) / b
来源：http://hz.gotoacloud.top/gtymiggaqm.html

[S52] C++：const 与 noexcept
来源：http://hz.yangfankeji.com/gtgtskdcxg.html

int size() const noexcept { return n_; }
来源：http://hz.jinghuilouyu.cn/gtlvyqobqx.html

[S53] C++：移动语义
来源：http://hz.yangfankeji.com/gtbknzmcde.html

std::vector<int> w = std::move(v);
来源：http://hz.jyoumei.cn/gtwbbasdai.html

[S54] C++：异常处理
来源：http://hz.shanyushiyangtech.top/gtozpipjzo.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.hongshengwenyu.top/gtyydxkupj.html

[S55] C++：结构化绑定
来源：http://hz.hfpthk.cn/gtrzpxprlu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.hywenlv.cn/gttidevecq.html

[S56] C++：optional
来源：http://hz.andypj.xyz/gtvwadjchr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.cqqwz.cn/gtevreosrc.html

[S57] C++：编译期常量
来源：http://hz.wangdashe.top/gtedmerirf.html

constexpr int N = 10;
来源：http://hz.jyoumei.cn/gttxjlqoxg.html

[S58] C++：命名空间
来源：http://hz.ppjwa.cn/gtvelujyvc.html

namespace ns { int f() { return 1; } }
来源：http://hz.0kj1m.cn/gtwhrdanxt.html

[S59] C++：静态断言
来源：http://hz.gzhubu.top/gtrilribdz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.shangyingyoupin.top/gtjrtgmogy.html

[S60] C++：遍历并删除元素
来源：http://hz.hnqzz.top/gtyiemltxy.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.wangshuangyany.cn/gtrlkzrtuv.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtbdsrplyy.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jiagoushi.top/gthnqnjldc.html

================================================================================
来源：http://hz.birdmap.top/gtltysoaze.html

[T01] Kotlin：Hello World
来源：http://hz.daxiang520.top/gtrgcagcbp.html

println("Hello")
来源：http://hz.yongpay.top/gtlslbdvhy.html

[T02] Kotlin：变量
来源：http://hz.316326.xyz/gtqbpphyye.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.xylfe.cn/gtklkawndc.html

[T03] Kotlin：字符串模板
来源：http://hz.chenzaomai.com/gtscpsnqst.html

"值: $b"
来源：http://hz.quarkkingdee.top/gtkgnxutdp.html

[T04] Kotlin：空安全
来源：http://hz.aibaodan.cn/gtrbtnvpom.html

val n: String? = null;  n?.length
来源：http://hz.xingfuxueyuan.xyz/gtbacmrawh.html

[T05] Kotlin：when 表达式
来源：http://hz.sxryk.cn/gtzrfpsara.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.fengsongda.top/gtlcmpccql.html

[T06] Kotlin：集合映射
来源：http://hz.yj20258.top/gtlwexdxbc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.kuanghao11.cn/gtaigbicnq.html

[T07] Kotlin：集合过滤
来源：http://hz.nwbrower.top/gtmbrwpnbh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.shanyushiyangkeji.top/gtkzaeltzv.html

[T08] Kotlin：数据类
来源：http://hz.tanke756.top/gtwmatkoke.html

data class User(val name: String, val age: Int)
来源：http://hz.chenzaomai.com/gttemueite.html


<!-- 参考信息 -->