代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zycfv.cn/gtvsexlvxd.html

[R10] 正则匹配
来源：http://hz.hnxiangtu.top/gtnminjjqv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.ivvv.top/gtkgtygkwl.html

[R11] case 多分支
来源：http://hz.yj202588.top/gtjhmlbnmh.html

case "$1" in
来源：http://hz.cheryme.top/gtnsdjakgm.html

start) echo "启动" ;;
来源：http://hz.ywan-chungtsiang.top/gtfbguvmqe.html

stop)  echo "停止" ;;
来源：http://hz.fengsongda.top/gtmtqexxpv.html

*)     echo "未知命令" ;;
来源：http://hz.jianghu66.top/gtztjsqagp.html

esac
来源：http://hz.hammf.cn/gtyxxfvrhq.html

[R12] for 遍历文件
来源：http://hz.ybcxt.top/gtlozqtmtv.html

for f in *.txt; do echo "$f"; done
来源：http://hz.shzxlz.cn/gtgvsvicks.html

[R13] for 计数循环
来源：http://hz.daria6918.cn/gtsjrvaxlq.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.pycfn.com/gtotngencl.html

[R14] C 风格 for
来源：http://hz.ehwqpu.com/gtlwjrtwmv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jyoumei.cn/gtsripvhfz.html

[R15] while 逐行读文件
来源：http://hz.wangshuangyany.cn/gtcedisvpq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.shangyingyoupin.top/gtrbnwboft.html

[R16] until 等待条件
来源：http://hz.zdqjudy.top/gthnyltuqi.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.pycfn.com/gtrzmaqosw.html

[R17] 数组定义与取值
来源：http://hz.cashguo.top/gtxzvztato.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.ehwqpu.com/gtcmvdrjin.html

[R18] 遍历数组
来源：http://hz.yangfankeji.com/gtilxaikri.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.shzxlz.cn/gtoeeyiftd.html

[R19] 数组长度
来源：http://hz.jqgfzy.top/gtnbagjpum.html

echo "${#arr[@]}"
来源：http://hz.feifeiyinyue.top/gtkwsgxoaw.html

[R20] 关联数组（字典）
来源：http://hz.fengsongda.top/gtqfqoqbhz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.sweek.top/gtrvglcaeb.html

[R21] 字符串长度
来源：http://hz.zhongyouzk.top/gtquvwpjid.html

echo "${#s}"
来源：http://hz.zhaomingkeji.xyz/gtaukfddsp.html

[R22] 截取子串
来源：http://hz.chenzaomai.com/gttvsmgfys.html

echo "${s:0:5}"
来源：http://hz.aibaodan.cn/gtkoidzyvx.html

[R23] 字符串替换
来源：http://hz.jqgufenzy.top/gtmzxhpdad.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.yanxiufei.cn/gtodhgupgy.html

[R24] 大小写转换
来源：http://hz.sxryk.cn/gtbowzloob.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.haohaochexian.top/gtjelmxyll.html

[R25] 去后缀 / 去前缀
来源：http://hz.ivvv.top/gtzxzujose.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.xylfe.cn/gteaxoksgi.html

[R26] 命令替换
来源：http://hz.wangdashe.top/gtbrhtwqvn.html

now=$(date +%F); echo "$now"
来源：http://hz.0kj1m.cn/gtjygrbags.html

[R27] 算术展开
来源：http://hz.hywenlv.cn/gtjugjqtxm.html

echo $((1 + 2 * 3))
来源：http://hz.kuanghao11.cn/gtpjcwemjs.html

[R28] 浮点运算
来源：http://hz.gogol.net.cn/gtjntyphek.html

echo "scale=2; 10/3" | bc
来源：http://hz.yuanzhike.top/gtxcqhqlpb.html

[R29] 定义函数
来源：http://hz.pycfn.com/gtssowhrwg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.havefunace.top/gtznkwsyez.html

[R30] 函数返回状态码
来源：http://hz.dashuyun.cn/gtazdrfcwy.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jinqigufen.top/gtvoqftxde.html

[R31] 局部变量
来源：http://hz.zhixingplan.top/gtyppsscki.html

f() { local x=1; echo "$x"; }
来源：http://hz.jinqigufen.top/gtwdzqteyc.html

[R32] 参数个数校验
来源：http://hz.xingfuxueyuan.xyz/gtdhkwvfet.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yuanzhike.top/gtjrdegopq.html

[R33] 捕获错误并提示行号
来源：http://hz.gotoacloud.top/gtziqomzcw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.gotoacloud.top/gtgbvxrnxg.html

[R34] 退出时清理
来源：http://hz.meibo888.top/gtvcgsrpuh.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.wangdashe.top/gtbpohkvbt.html

[R35] 后台执行并等待
来源：http://hz.zhoulong.xyz/gtcjxkutkb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.shanyushiyangkeji.top/gtrjhnpexp.html

[R36] 并发执行多个任务
来源：http://hz.smart0.xyz/gtrguhvscq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yuxming.cn/gtnfhtktjj.html

[R37] 把输出赋给变量
来源：http://hz.sweek.top/gtakernkha.html

files=$(ls -1)
来源：http://hz.ppjwa.cn/gtrhzekcik.html

[R38] 管道串联
来源：http://hz.gzhubu.top/gtmdrnluww.html

cat a.txt | grep -i error | wc -l
来源：http://hz.ivvv.top/gtashflbhh.html

[R39] 重定向标准输出与错误
来源：http://hz.jyoumei.cn/gtqnhwwpfu.html

cmd > out.log 2>&1
来源：http://hz.guannengcc.top/gtzwbfroob.html

[R40] 追加写日志
来源：http://hz.guannengcc.top/gtujleqsdx.html

echo "log" >> out.log
来源：http://hz.yvedp.cn/gtrlgdernp.html

[R41] 丢弃输出
来源：http://hz.birdmap.top/gtqeskaibu.html

cmd >/dev/null 2>&1
来源：http://hz.yonumen.top/gtwflqaqbe.html

[R42] 输入重定向
来源：http://hz.hammf.cn/gtabjkojlc.html

wc -l < a.txt
来源：http://hz.yanxiufei.cn/gtabhjfpqm.html

[R43] 按名字查找文件
来源：http://hz.svipenyu.cn/gtvhxninie.html

find . -name "*.log" -type f
来源：http://hz.xuetiantiany.cn/gtvbttvhnd.html

[R44] 按修改时间查找
来源：http://hz.vqdsnc.cn/gtanlidlpa.html

find . -mtime -7 -type f
来源：http://hz.jianghu66.top/gtfhkjlkwa.html

[R45] 批量删除
来源：http://hz.cheryme.top/gtczyqenjc.html

find . -name "*.tmp" -delete
来源：http://hz.hfpthk.cn/gtqdmdstyu.html

[R46] 递归替换文件内容
来源：http://hz.andypj.xyz/gtjthsexlu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.smart0.xyz/gtpoqksqgv.html

[R47] sed 单行替换
来源：http://hz.redwolf501.top/gtzktbtfrf.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.iojbl.cn/gtlfwyukmp.html

[R48] awk 取指定列
来源：http://hz.zhaomingkeji.xyz/gtnejzsnas.html

awk '{print $1, $3}' a.txt
来源：http://hz.xylfe.cn/gtvplfhnfr.html

[R49] awk 带条件
来源：http://hz.fengsongda.top/gtymxruxwr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.jinqigfzy.top/gtczghktqc.html

[R50] awk 求和
来源：http://hz.yangfankeji.com/gthyqdoplj.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.hnqzz.top/gtyqaoajjd.html

[R51] 排序去重取前几
来源：http://hz.birdmap.top/gtquoyltsg.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.cashguo.top/gtjjofmtlo.html

[R52] 统计行数
来源：http://hz.gogol.net.cn/gtusqaetze.html

wc -l a.txt
来源：http://hz.nwbrower.top/gtorqxsxiz.html

[R53] 查看文件头与实时尾
来源：http://hz.xuetiantiany.cn/gthfucvdmh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.xingfuxueyuan.xyz/gtscwmfjox.html

[R54] 比较两个文件
来源：http://hz.bjfxy.top/gtvhgmktmv.html

diff a.txt b.txt
来源：http://hz.shanyushiyangkeji.top/gtvujqrhyr.html

[R55] 压缩与解压
来源：http://hz.havefunace.top/gtzycaoeae.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.vqdsnc.cn/gtvqgysklg.html

[R56] 远程拷贝
来源：http://hz.nwbrower.top/gtyqwivamc.html

scp file user@host:/path/
来源：http://hz.feifeiyinyue.top/gtflrtxpjj.html

[R57] 远程执行命令
来源：http://hz.ybcxt.top/gtdbymysoj.html

ssh user@host 'uptime'
来源：http://hz.pycfn.com/gtzooclwoq.html

[R58] 下载文件
来源：http://hz.yueranfly.top/gtqweixqpd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.zhixingplan.top/gtxjmkotoq.html

[R59] 发 POST JSON
来源：http://hz.xziqi.cn/gtrdalwetv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yanxiufei.cn/gtqwfkzsaz.html

[R60] 只看 HTTP 状态码
来源：http://hz.hammf.cn/gtovkzjxwm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.xingfuxueyuan.xyz/gtnwhseuzt.html

[R61] 磁盘占用
来源：http://hz.guowangkeji.top/gtcieqkprb.html

df -h;  du -sh *
来源：http://hz.yj20258.top/gtpxohbufj.html

[R62] 找最占空间的文件
来源：http://hz.cheryme.top/gtzbjunhtw.html

du -ah . | sort -rh | head -10
来源：http://hz.ywan-chungtsiang.top/gtpowwbizn.html

[R63] 内存与进程
来源：http://hz.yuanzhike.top/gtefrbgxoi.html

free -h;  ps aux | grep nginx
来源：http://hz.zdqjudy.top/gttouhxtfi.html

[R64] 结束进程
来源：http://hz.gotoacloud.top/gttszltiym.html

kill -9 $(pgrep -f app.py)
来源：http://hz.shzxlz.cn/gtbyxjzzwt.html

[R65] 查看端口占用
来源：http://hz.hnqzz.top/gtkheyqnpd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.zhoulong.xyz/gttgvoktmh.html

[R66] 定时任务
来源：http://hz.zycfv.cn/gtebhxtizw.html

crontab -e;  crontab -l
来源：http://hz.yongpay.top/gtefpnalgk.html

[R67] 生成随机十六进制串
来源：http://hz.gaohongyu789.top/gtstkmfwki.html

openssl rand -hex 16
来源：http://hz.ydzc1.top/gtfyrkzavz.html

[R68] 计算文件校验值
来源：http://hz.9152youxi.cn/gtaavlpcev.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.fzhhl.top/gtmdkzktah.html

[R69] 生成随机密码
来源：http://hz.xinyue.icu/gttndhlepc.html

head -c 16 /dev/urandom | base64
来源：http://hz.hywenlv.cn/gtjuqpudzp.html

[R70] 时间戳与互转
来源：http://hz.sufxvd.cn/gtfcjkqlsa.html

date +%s;  date -d @1700000000
来源：http://hz.aibaodan.cn/gtnyendnzy.html

[R71] 日期格式化
来源：http://hz.fzhhl.top/gtlacixbez.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.cqqwz.cn/gtjrgceigj.html

[R72] 等待端口就绪
来源：http://hz.ppjwa.cn/gtemgnbnyw.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.bjfxy.top/gtyqtwgqch.html

[R73] 分割大日志
来源：http://hz.ehwqpu.com/gtmmkrwihn.html

split -l 1000 big.log part_
来源：http://hz.bjfxy.top/gtxbwxrbzk.html

[R74] 批量重命名
来源：http://hz.gogol.net.cn/gtqhtdlpru.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.vqdsnc.cn/gttroimvjk.html

[R75] 导出环境变量
来源：http://hz.jianghu66.top/gtpsbzwrdf.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.hongshengwenyu.top/gtprzdxveo.html

[R76] 使用临时文件
来源：http://hz.jqgufenzy.top/gtwzecqxrn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhoulong.xyz/gtsqedkhcc.html

[R77] 读取用户输入
来源：http://hz.jinqigfzy.top/gthfmbomqk.html

read -rp "请输入: " ans
来源：http://hz.jinyuanbaomall.cn/gthfrfhryu.html

[R78] 交互式菜单
来源：http://hz.guannengcc.top/gtfhkcqllq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yj20258888.top/gtcyehdcqi.html

[R79] 解析命令行选项
来源：http://hz.zhoulong.xyz/gtfcwqrnhb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.xingfuxueyuan.xyz/gtsvnrjddr.html

[R80] 查看脚本执行耗时
来源：http://hz.zdqjudy.top/gtfuipanmo.html

time ./run.sh
来源：http://hz.andypj.xyz/gtubbusvhw.html

================================================================================
来源：http://hz.hysaishi.cn/gtyhcjxzox.html

S. C / C++ 专题
来源：http://hz.yvedp.cn/gtqzakmzqo.html

================================================================================
来源：http://hz.sweek.top/gtuevjcnjw.html

[S01] C：Hello World
来源：http://hz.xziqi.cn/gtvwphqkbl.html

#include <stdio.h>
来源：http://hz.gaohongyu789.top/gtdhirbzxa.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jyoumei.cn/gtrymbgpgv.html

[S02] C：变量与格式化输出
来源：http://hz.gaohongyu789.top/gtxbrancgz.html

int a = 10; printf("%d\n", a);
来源：http://hz.feifeiyinyue.top/gtgvztwmzh.html

[S03] C：读入整数
来源：http://hz.shuidangran.top/gtdcxgjhfg.html

int x; scanf("%d", &x);
来源：http://hz.gaohongyu789.top/gtyonuvbra.html

[S04] C：字符串复制
来源：http://hz.zdqjudy.top/gtfvlqidgz.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.hysaishi.cn/gtpajcfviu.html

[S05] C：字符串长度
来源：http://hz.tanke756.top/gtopcvkiqm.html

strlen(s)
来源：http://hz.jinyuanbaomall.cn/gtubisosjj.html

[S06] C：字符串比较
来源：http://hz.zhaomingkeji.xyz/gtvrunjzsb.html

strcmp(a, b) == 0
来源：http://hz.tianlin.xyz/gtiqupmhrr.html

[S07] C：数组遍历求和
来源：http://hz.0kj1m.cn/gtrrodpfuv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jlsjyb.cn/gtcjptydga.html

[S08] C：动态内存分配与释放
来源：http://hz.feifeiyinyue.top/gtcdwfqmda.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.xingfuxueyuan.xyz/gtauuohmnv.html

[S09] C：结构体定义与初始化
来源：http://hz.tanke756.top/gtagoxsduq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.ivvv.top/gtcmeiwmfp.html

[S10] C：指针与解引用
来源：http://hz.feifeiyinyue.top/gtcfwvzelp.html

int *p = &a;  *p = 5;
来源：http://hz.yuxming.cn/gtpurzeaon.html

[S11] C：逐行读文件
来源：http://hz.ivvv.top/gtfemzrlcy.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.c1oappe.top/gteknqidtl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.zhixingplan.top/gtkncdnkon.html

fclose(f);
来源：http://hz.hnqzz.top/gtxwykaeep.html

[S12] C：写文件
来源：http://hz.xuetiantiany.cn/gtqhokvtvm.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.cucudq.cn/gtlmfvfovk.html

[S13] C：宏定义
来源：http://hz.nanxinkj.top/gttxhulcno.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.gaohongyu789.top/gtohcibbnb.html

[S14] C：枚举
来源：http://hz.feifeiyinyue.top/gtuqopoiwn.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.jinqigfzy.top/gtfcvoyttv.html

[S15] C：类型转换
来源：http://hz.yanxiufei.cn/gtxjcpyunw.html

(double) a / b
来源：http://hz.wangshuangyany.cn/gtjwfndchl.html

[S16] C：位操作置位
来源：http://hz.svipenyu.cn/gtyprcpjkl.html

x |= (1 << 3);
来源：http://hz.ydjk.org.cn/gtdjslyqpg.html

[S17] C：安全拼接字符串
来源：http://hz.sweek.top/gtofqdiawg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.ydjk.org.cn/gthcmiqcje.html

[S18] C：命令行参数
来源：http://hz.yj202588.top/gtmuaxbnds.html

int main(int argc, char **argv)
来源：http://hz.meibo888.top/gtdacqnzeg.html

[S19] C：快速排序
来源：http://hz.pycfn.com/gttmpcfbit.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.wangshuangyany.cn/gtpofabpqj.html

[S20] C：二分查找
来源：http://hz.yonumen.top/gtekajjwzd.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.ivvv.top/gtmjdazpfz.html

[S21] C：字符类别判断
来源：http://hz.wangshuangyany.cn/gtndxcafoj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.pengpengdd.cyou/gtrcowakcv.html

[S22] C：字符串转数字
来源：http://hz.shangyingyoupin.top/gtvisgsopt.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.cdnleiting.top/gtmolaxbdw.html

[S23] C：随机数
来源：http://hz.svipenyu.cn/gtioectndp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.jinyuanbaomall.cn/gthxzenjev.html

[S24] C：获取本地时间
来源：http://hz.yanxiufei.cn/gtxnmstkte.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.dianchejie.cn/gtkcnxrjai.html

[S25] C：内存拷贝
来源：http://hz.yj20258.top/gtxeutvfjo.html

memcpy(dst, src, n);
来源：http://hz.quarkkingdee.top/gtpvwyrqod.html

[S26] C：内存清零
来源：http://hz.sufxvd.cn/gtdpggcpis.html

memset(a, 0, sizeof a);
来源：http://hz.jianghu66.top/gtejbnvkvx.html

[S27] C：定义常量
来源：http://hz.xingfuxueyuan.xyz/gtekruslqm.html

const double PI = 3.14159;
来源：http://hz.tianlin.xyz/gtdnqowmwt.html

[S28] C：静态变量
来源：http://hz.yvedp.cn/gtvywyrqop.html

static int counter = 0;
来源：http://hz.dianchejie.cn/gtuarjotcs.html

[S29] C：变参函数
来源：http://hz.quarkkingdee.top/gtvpsqkgzk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.smart0.xyz/gtelxnlbue.html

[S30] C：头文件保护
来源：http://hz.jlsjyb.cn/gtfqnlajnp.html

#ifndef X_H
来源：http://hz.yvedp.cn/gtcqaxmrks.html

#define X_H
来源：http://hz.iojbl.cn/gtqhbqyeug.html

#endif
来源：http://hz.yvedp.cn/gtxognrzlw.html

[S31] C++：Hello World
来源：http://hz.hnqzz.top/gtrmbbijqy.html

#include <iostream>
来源：http://hz.pycfn.com/gtwcybfccs.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.cdnleiting.top/gthfnamaht.html

[S32] C++：字符串
来源：http://hz.havefunace.top/gtbboqrpbs.html

std::string s = "hi";  s += "!";
来源：http://hz.chenjidiqi.icu/gtbimbqfcu.html

[S33] C++：vector 增删
来源：http://hz.jyoumei.cn/gtvokxvepv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yuxming.cn/gtyegpcjga.html

[S34] C++：遍历 vector
来源：http://hz.wangdashe.top/gtaijfnzte.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.feifeiyinyue.top/gtnedfcanw.html

[S35] C++：map
来源：http://hz.zhijiandao.cn/gtubzdycqn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.tanke756.top/gtrusbkdcg.html

[S36] C++：unordered_map
来源：http://hz.nwbrower.top/gtjteykhwk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.quarkkingdee.top/gttfqljuls.html

[S37] C++：set
来源：http://hz.jinyuanbaomall.cn/gtpluowkzj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.tian-w.cn/gtakfdmsdk.html

[S38] C++：排序
来源：http://hz.kuanghao11.cn/gtnsqzjltb.html

std::sort(v.begin(), v.end());
来源：http://hz.yuxming.cn/gtbihnimeb.html

[S39] C++：自定义比较器排序
来源：http://hz.9152youxi.cn/gtjfbdcygc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.gogol.net.cn/gtegwtfhkt.html

[S40] C++：查找元素
来源：http://hz.tian-w.cn/gtevakyalu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.cashguo.top/gtunmjnitu.html

[S41] C++：类与构造函数
来源：http://hz.nwbrower.top/gtezacqbul.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.jyoumei.cn/gtpvtlopsj.html

[S42] C++：继承与虚函数
来源：http://hz.ydjk.org.cn/gtarjnccuf.html

class B : public Base { public: void f() override {} };
来源：http://hz.cashguo.top/gtjmkxoyvj.html

[S43] C++：智能指针
来源：http://hz.shzxlz.cn/gtpebheoiv.html

auto p = std::make_unique<int>(5);
来源：http://hz.ehwqpu.com/gtsbidzyye.html

[S44] C++：引用传参
来源：http://hz.guowangkeji.top/gtdvhpcons.html

void inc(int &x) { ++x; }
来源：http://hz.chenlongwang.top/gtipxkbwcr.html

[S45] C++：lambda
来源：http://hz.jinqigufen.top/gtpreqobwn.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.xinyue.icu/gtcmmoqdha.html

[S46] C++：函数模板
来源：http://hz.ywan-chungtsiang.top/gtbcihocxm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.ywan-chungtsiang.top/gtpjiuhqyi.html

[S47] C++：结构化绑定遍历
来源：http://hz.quarkkingdee.top/gtdappepbl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.hongshengwenyu.top/gtziypgspd.html

[S48] C++：逐行读文件
来源：http://hz.jinqigufen.top/gtckzeosww.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.xylfe.cn/gtfhbqpqbi.html

while (std::getline(in, line)) { }
来源：http://hz.yvedp.cn/gthelphmdh.html

[S49] C++：写文件
来源：http://hz.quarkkingdee.top/gtyjdauyev.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.meibo888.top/gtgljhtpmk.html

[S50] C++：格式化数字
来源：http://hz.haohaochexian.top/gtzhqarspl.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.haohaochexian.top/gtsmmhcbox.html

[S51] C++：显式类型转换
来源：http://hz.yongpay.top/gtgxzjpbig.html

static_cast<double>(a) / b
来源：http://hz.ppjwa.cn/gtvnmqzbcd.html

[S52] C++：const 与 noexcept
来源：http://hz.chenzaomai.com/gtlsxxluei.html

int size() const noexcept { return n_; }
来源：http://hz.cucudq.cn/gtxxemjphy.html

[S53] C++：移动语义
来源：http://hz.yvedp.cn/gtvbeadbbq.html

std::vector<int> w = std::move(v);
来源：http://hz.hongshengwenyu.top/gtessczjlx.html

[S54] C++：异常处理
来源：http://hz.daxiang520.top/gtaqyvjpec.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.daxiang520.top/gtklmpthqy.html

[S55] C++：结构化绑定
来源：http://hz.cqqwz.cn/gtegiuasbu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.cucudq.cn/gtxeodazgv.html

[S56] C++：optional
来源：http://hz.smart0.xyz/gtplvetyen.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.fzhhl.top/gteworpium.html

[S57] C++：编译期常量
来源：http://hz.redwolf501.top/gtergrgjus.html

constexpr int N = 10;
来源：http://hz.fzhhl.top/gtquzsthya.html

[S58] C++：命名空间
来源：http://hz.zhijiandao.cn/gtyotdylpn.html

namespace ns { int f() { return 1; } }
来源：http://hz.shuidangran.top/gtjtxyyrrc.html

[S59] C++：静态断言
来源：http://hz.vqdsnc.cn/gtkzalfuew.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.yangfankeji.com/gtzleimhoy.html

[S60] C++：遍历并删除元素
来源：http://hz.shuidangran.top/gtkaqoaopd.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jinghuilouyu.cn/gtisstcjkw.html

================================================================================
来源：http://hz.shzxlz.cn/gtetvblaez.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zdqjudy.top/gtplsiwpgk.html

================================================================================
来源：http://hz.wangdashe.top/gtlawczygc.html

[T01] Kotlin：Hello World
来源：http://hz.xylfe.cn/gtueaufavt.html

println("Hello")
来源：http://hz.yj202588.top/gtzenrpyuh.html

[T02] Kotlin：变量
来源：http://hz.yvedp.cn/gtbprbcgwn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.sweek.top/gtrxhadahg.html

[T03] Kotlin：字符串模板
来源：http://hz.birdmap.top/gtscdtxafv.html

"值: $b"
来源：http://hz.shzxlz.cn/gtozjwfvav.html

[T04] Kotlin：空安全
来源：http://hz.sweek.top/gtfyaojdxb.html

val n: String? = null;  n?.length
来源：http://hz.jinqigfzy.top/gtfbsnpklh.html

[T05] Kotlin：when 表达式
来源：http://hz.yangfankeji.com/gticlrinwd.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yongpay.top/gthydnoslm.html

[T06] Kotlin：集合映射
来源：http://hz.guowangkeji.top/gttburonpj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.hammf.cn/gtzyhqgmvh.html

[T07] Kotlin：集合过滤
来源：http://hz.yj20258888.top/gttlwwezap.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.xinyue.icu/gtesqseopf.html

[T08] Kotlin：数据类
来源：http://hz.chenlongwang.top/gttwopszhv.html

data class User(val name: String, val age: Int)
来源：http://hz.gotoacloud.top/gtzmrcnvuw.html

[T09] Kotlin：扩展函数
来源：http://hz.yvedp.cn/gtspblyikm.html

fun String.exclaim() = this + "!"
来源：http://hz.bjfxy.top/gteuwlxldf.html

[T10] Kotlin：默认参数
来源：http://hz.tianlin.xyz/gtzdrjnswx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jianghu66.top/gtngrvural.html


<!-- 参考信息 -->