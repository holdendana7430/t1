代发 wailian999

case "$1" in
来源：http://hz.xuanzx.com/gtotodmfyp.html

start) echo "启动" ;;
来源：http://hz.jinghuilouyu.cn/gtpvbwunps.html

stop)  echo "停止" ;;
来源：http://hz.zhiwuduotai.top/gtjqqrjgna.html

*)     echo "未知命令" ;;
来源：http://hz.zhijiandao.cn/gtvkxaundo.html

esac
来源：http://hz.zhongyouzk.top/gthjcbsdjp.html

[R12] for 遍历文件
来源：http://hz.bjfxy.top/gtulmtqapg.html

for f in *.txt; do echo "$f"; done
来源：http://hz.zdqjudy.top/gtqsmhiymc.html

[R13] for 计数循环
来源：http://hz.yangfankeji.com/gtazesnlod.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.hysaishi.cn/gthgmnhxyr.html

[R14] C 风格 for
来源：http://hz.snrcjt.cn/gttbsrizfm.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.tanke756.top/gtsncjaljr.html

[R15] while 逐行读文件
来源：http://hz.jinyuanbaomall.cn/gtttlwtbzl.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.cqqwz.cn/gtaogwwlsu.html

[R16] until 等待条件
来源：http://hz.jinyuanbaomall.cn/gtvfwithvk.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.daria6918.cn/gtmpahsgco.html

[R17] 数组定义与取值
来源：http://hz.sufxvd.cn/gtvgaxrtpm.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.sxryk.cn/gtspesgrpy.html

[R18] 遍历数组
来源：http://hz.52xcode.cn/gtejckwarf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.shanyushiyangtech.top/gtmzqklpqf.html

[R19] 数组长度
来源：http://hz.mhx1999.top/gtshqxnuzl.html

echo "${#arr[@]}"
来源：http://hz.yuanzhike.top/gtmvhxppug.html

[R20] 关联数组（字典）
来源：http://hz.cdnleiting.top/gtwrjokdjx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.ehwqpu.com/gtdmpsfiyj.html

[R21] 字符串长度
来源：http://hz.shanyushiyangkeji.top/gtzkwtmmqb.html

echo "${#s}"
来源：http://hz.xuetiantiany.cn/gtkeldkaos.html

[R22] 截取子串
来源：http://hz.yongpay.top/gtrtqjplib.html

echo "${s:0:5}"
来源：http://hz.jianghu66.top/gtdtxfgzww.html

[R23] 字符串替换
来源：http://hz.guowangkeji.top/gtwseqxorf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.ivvv.top/gttgawqrcr.html

[R24] 大小写转换
来源：http://hz.havefunace.top/gtpryugjai.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.nwbrower.top/gtttzdkmbz.html

[R25] 去后缀 / 去前缀
来源：http://hz.xylfe.cn/gtudzoxthz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yanxiufei.cn/gtsuyknfqr.html

[R26] 命令替换
来源：http://hz.vqdsnc.cn/gtxwywnmws.html

now=$(date +%F); echo "$now"
来源：http://hz.shzxlz.cn/gtntpttqcc.html

[R27] 算术展开
来源：http://hz.aizwys.cn/gtggpfkylo.html

echo $((1 + 2 * 3))
来源：http://hz.smart0.xyz/gtydbaoajr.html

[R28] 浮点运算
来源：http://hz.shzxlz.cn/gtielknnze.html

echo "scale=2; 10/3" | bc
来源：http://hz.nanxinkj.top/gtcxzyysuo.html

[R29] 定义函数
来源：http://hz.wangshuangyany.cn/gtynnmippg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.sysykeji.top/gtfqcbvvzq.html

[R30] 函数返回状态码
来源：http://hz.gzhubu.top/gtjznepyty.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.zhaomingkeji.xyz/gtkfaxqtcs.html

[R31] 局部变量
来源：http://hz.wangshuangyany.cn/gtebmysvwu.html

f() { local x=1; echo "$x"; }
来源：http://hz.yuanzhike.top/gtevrzxfvl.html

[R32] 参数个数校验
来源：http://hz.hnxiangtu.top/gtyjcvemif.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.xuanzx.com/gthuanfijr.html

[R33] 捕获错误并提示行号
来源：http://hz.zhijiandao.cn/gtaekuuyhg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jinqigufen.top/gtwnctczln.html

[R34] 退出时清理
来源：http://hz.zhixingplan.top/gtxjbqyikj.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jinqigfzy.top/gtgulpghub.html

[R35] 后台执行并等待
来源：http://hz.zhengqikj.top/gtgdfgiczr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.andypj.xyz/gtkboowgwy.html

[R36] 并发执行多个任务
来源：http://hz.guowangkeji.top/gtboooihpo.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yvedp.cn/gtrvbaoiej.html

[R37] 把输出赋给变量
来源：http://hz.hnqzz.top/gthafsasig.html

files=$(ls -1)
来源：http://hz.9152youxi.cn/gtidxoomme.html

[R38] 管道串联
来源：http://hz.xuetiantiany.cn/gtivgystqv.html

cat a.txt | grep -i error | wc -l
来源：http://hz.ivvv.top/gtbvdrzrwl.html

[R39] 重定向标准输出与错误
来源：http://hz.shuidangran.top/gtfkiuztef.html

cmd > out.log 2>&1
来源：http://hz.birdmap.top/gtyoemdngj.html

[R40] 追加写日志
来源：http://hz.haohaochexian.top/gtgequqeog.html

echo "log" >> out.log
来源：http://hz.xinyue.icu/gtmovoiwrg.html

[R41] 丢弃输出
来源：http://hz.quarkkingdee.top/gtnlgrprws.html

cmd >/dev/null 2>&1
来源：http://hz.zhoulong.xyz/gtttrglwqp.html

[R42] 输入重定向
来源：http://hz.jinghuilouyu.cn/gtewxivnjj.html

wc -l < a.txt
来源：http://hz.xuetiantiany.cn/gteoxvnxbv.html

[R43] 按名字查找文件
来源：http://hz.ybcxt.top/gtssstkusx.html

find . -name "*.log" -type f
来源：http://hz.guannengcc.top/gtwiwimzma.html

[R44] 按修改时间查找
来源：http://hz.0kj1m.cn/gtiqidrebd.html

find . -mtime -7 -type f
来源：http://hz.yangfankeji.com/gtcijaairl.html

[R45] 批量删除
来源：http://hz.dianchejie.cn/gtapuztchg.html

find . -name "*.tmp" -delete
来源：http://hz.bjfxy.top/gtsrhlyboe.html

[R46] 递归替换文件内容
来源：http://hz.cqqwz.cn/gtvozcjpzs.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.guannengcc.top/gtpkurqyxk.html

[R47] sed 单行替换
来源：http://hz.ydjk.org.cn/gtotjdejqm.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.jianghu66.top/gtcxpugyyh.html

[R48] awk 取指定列
来源：http://hz.tianlin.xyz/gtiwogbpyj.html

awk '{print $1, $3}' a.txt
来源：http://hz.shzxlz.cn/gteasfeyom.html

[R49] awk 带条件
来源：http://hz.zycfv.cn/gtvtjroqei.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.ehwqpu.com/gtsdbffrwf.html

[R50] awk 求和
来源：http://hz.cheryme.top/gtatpwfbbi.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.aibaodan.cn/gtcapumjsa.html

[R51] 排序去重取前几
来源：http://hz.smart0.xyz/gtrgzeghkb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.wangshuangyany.cn/gteqwsqeuv.html

[R52] 统计行数
来源：http://hz.dianchejie.cn/gtuobmoviu.html

wc -l a.txt
来源：http://hz.wangshuangyany.cn/gtogjcibpv.html

[R53] 查看文件头与实时尾
来源：http://hz.sxryk.cn/gtitxqdeww.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.cqqwz.cn/gtgrkxfzbp.html

[R54] 比较两个文件
来源：http://hz.chenzaomai.com/gthwsrxhhd.html

diff a.txt b.txt
来源：http://hz.birdmap.top/gttcyrsjzl.html

[R55] 压缩与解压
来源：http://hz.yangfankeji.com/gtprihqclr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.jinghuilouyu.cn/gtikeypnjy.html

[R56] 远程拷贝
来源：http://hz.jinqigfzy.top/gtmmkhwtyo.html

scp file user@host:/path/
来源：http://hz.svipenyu.cn/gtjsfiympc.html

[R57] 远程执行命令
来源：http://hz.zdqjudy.top/gterurzqtj.html

ssh user@host 'uptime'
来源：http://hz.tianlin.xyz/gtdznfyzze.html

[R58] 下载文件
来源：http://hz.shzxlz.cn/gtxvtpyepn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.fzhhl.top/gtlhkbzaeq.html

[R59] 发 POST JSON
来源：http://hz.tanke756.top/gtmmeclnyh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jinghuilouyu.cn/gtokgjaavh.html

[R60] 只看 HTTP 状态码
来源：http://hz.bjfxy.top/gtajdwmhsf.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.ydzc1.top/gtjgrhfutp.html

[R61] 磁盘占用
来源：http://hz.ydjk.org.cn/gtonyfqymj.html

df -h;  du -sh *
来源：http://hz.tianlin.xyz/gttqobbwnf.html

[R62] 找最占空间的文件
来源：http://hz.wangshuangyany.cn/gtpgssgusk.html

du -ah . | sort -rh | head -10
来源：http://hz.nanxuanxn.top/gtardlwoie.html

[R63] 内存与进程
来源：http://hz.shanyushiyangkeji.top/gtixxeoeot.html

free -h;  ps aux | grep nginx
来源：http://hz.cucudq.cn/gtoyndwiue.html

[R64] 结束进程
来源：http://hz.redwolf501.top/gtlyhglbqq.html

kill -9 $(pgrep -f app.py)
来源：http://hz.sufxvd.cn/gtprzosjwo.html

[R65] 查看端口占用
来源：http://hz.cqqwz.cn/gtbsjzvadz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.nwbrower.top/gtfaynlopx.html

[R66] 定时任务
来源：http://hz.hongshengwenyu.top/gtqznfeemd.html

crontab -e;  crontab -l
来源：http://hz.zhijiandao.cn/gtmandunzh.html

[R67] 生成随机十六进制串
来源：http://hz.iojbl.cn/gtcynygltl.html

openssl rand -hex 16
来源：http://hz.jyoumei.cn/gtrawwcsst.html

[R68] 计算文件校验值
来源：http://hz.dianchejie.cn/gtdxbeyccl.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.9152youxi.cn/gthjsazawr.html

[R69] 生成随机密码
来源：http://hz.aizwys.cn/gtxejnjhjp.html

head -c 16 /dev/urandom | base64
来源：http://hz.tian-w.cn/gtqlxiqtun.html

[R70] 时间戳与互转
来源：http://hz.jlsjyb.cn/gtjnepwefm.html

date +%s;  date -d @1700000000
来源：http://hz.zhiwuduotai.top/gtkdgsgtrj.html

[R71] 日期格式化
来源：http://hz.jianghu66.top/gtvnvuyijw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.cqqwz.cn/gtdrosxjgz.html

[R72] 等待端口就绪
来源：http://hz.hfpthk.cn/gtcvhandqq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.52xcode.cn/gtbeanriuo.html

[R73] 分割大日志
来源：http://hz.yj202588.top/gtapjervax.html

split -l 1000 big.log part_
来源：http://hz.hywenlv.cn/gtgdhiadwl.html

[R74] 批量重命名
来源：http://hz.shanyushiyangkeji.top/gthameewbf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.chenlongwang.top/gtcrfjbyxt.html

[R75] 导出环境变量
来源：http://hz.vqdsnc.cn/gturpzmcqn.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yueranfly.top/gtcshxfjsb.html

[R76] 使用临时文件
来源：http://hz.ehwqpu.com/gtwjhunhfo.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.ybcxt.top/gtbrpfwaor.html

[R77] 读取用户输入
来源：http://hz.gotoacloud.top/gtnwvonmoo.html

read -rp "请输入: " ans
来源：http://hz.svipenyu.cn/gtzmpnhnym.html

[R78] 交互式菜单
来源：http://hz.zhoulong.xyz/gtifxlawxy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.zhixingplan.top/gtuxelcaya.html

[R79] 解析命令行选项
来源：http://hz.yonumen.top/gtjlssvtuz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jyoumei.cn/gtuufhkyay.html

[R80] 查看脚本执行耗时
来源：http://hz.sysykeji.top/gtgvtgpspu.html

time ./run.sh
来源：http://hz.xuanzx.com/gtpswfgoqh.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtlnwlimml.html

S. C / C++ 专题
来源：http://hz.shanyushiyangkeji.top/gtoedmibkp.html

================================================================================
来源：http://hz.yanxiufei.cn/gtfxhtruuh.html

[S01] C：Hello World
来源：http://hz.feifeiyinyue.top/gthdvrrqif.html

#include <stdio.h>
来源：http://hz.cdnleiting.top/gtjrblsxtl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.vqdsnc.cn/gtufgmttnt.html

[S02] C：变量与格式化输出
来源：http://hz.jqgufenzy.top/gtcesbsqms.html

int a = 10; printf("%d\n", a);
来源：http://hz.tanke756.top/gtknvkaqgy.html

[S03] C：读入整数
来源：http://hz.cheryme.top/gtqbyqzkjk.html

int x; scanf("%d", &x);
来源：http://hz.ppjwa.cn/gtmcbeggze.html

[S04] C：字符串复制
来源：http://hz.feifeiyinyue.top/gtkvomeafd.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.mhx1999.top/gtvgoryfck.html

[S05] C：字符串长度
来源：http://hz.hywenlv.cn/gtphjxxxzj.html

strlen(s)
来源：http://hz.jinghuilouyu.cn/gtywojytiw.html

[S06] C：字符串比较
来源：http://hz.zhongyouzk.top/gtpiusumum.html

strcmp(a, b) == 0
来源：http://hz.tanke756.top/gtgluacdrr.html

[S07] C：数组遍历求和
来源：http://hz.0kj1m.cn/gtdtjhophm.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.tian-w.cn/gtfiqnvoqp.html

[S08] C：动态内存分配与释放
来源：http://hz.wangshuangyany.cn/gtdiemksyh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yj20258.top/gtjkhrtyuj.html

[S09] C：结构体定义与初始化
来源：http://hz.dianchejie.cn/gtvzajnsmh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.snrcjt.cn/gtpetlvsfz.html

[S10] C：指针与解引用
来源：http://hz.gogol.net.cn/gtejonhqhf.html

int *p = &a;  *p = 5;
来源：http://hz.sysykeji.top/gtgarcslfw.html

[S11] C：逐行读文件
来源：http://hz.hongshengwenyu.top/gtenkvjqmm.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.9152youxi.cn/gtzatptxwy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.chenzaomai.com/gtpvsyuriy.html

fclose(f);
来源：http://hz.9152youxi.cn/gtapcuznxe.html

[S12] C：写文件
来源：http://hz.gotoacloud.top/gtjxdujfeb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.sxryk.cn/gtlwaedykq.html

[S13] C：宏定义
来源：http://hz.andypj.xyz/gtdhcokwzz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.daxiang520.top/gtazvzlibk.html

[S14] C：枚举
来源：http://hz.jqgfzy.top/gtkannnryq.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.ivvv.top/gtxmbthmvc.html

[S15] C：类型转换
来源：http://hz.cheryme.top/gtbcobprsw.html

(double) a / b
来源：http://hz.ivvv.top/gthlxlnncl.html

[S16] C：位操作置位
来源：http://hz.0kj1m.cn/gtecrsbztl.html

x |= (1 << 3);
来源：http://hz.yonumen.top/gtqhcqdefv.html

[S17] C：安全拼接字符串
来源：http://hz.jiagoushi.top/gtgxgbowqx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.daria6918.cn/gtnupvjkwn.html

[S18] C：命令行参数
来源：http://hz.havefunace.top/gtizaxnjon.html

int main(int argc, char **argv)
来源：http://hz.nwbrower.top/gtungxream.html

[S19] C：快速排序
来源：http://hz.aibaodan.cn/gtgbrxtpve.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.0kj1m.cn/gtezsuubky.html

[S20] C：二分查找
来源：http://hz.316326.xyz/gtmqinuges.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zycfv.cn/gtmmrwazdw.html

[S21] C：字符类别判断
来源：http://hz.yuanzhike.top/gtfyzipvck.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.hammf.cn/gtdyqegkom.html

[S22] C：字符串转数字
来源：http://hz.tian-w.cn/gtmngqnfrd.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.ybcxt.top/gtfbvedwvg.html

[S23] C：随机数
来源：http://hz.fzhhl.top/gteysoupiv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.andypj.xyz/gtphqxezpj.html

[S24] C：获取本地时间
来源：http://hz.jqgfzy.top/gttnvvlcwt.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yj20258888.top/gttxwaojva.html

[S25] C：内存拷贝
来源：http://hz.zhaomingkeji.xyz/gtkvwhyutk.html

memcpy(dst, src, n);
来源：http://hz.hongshengwenyu.top/gtndqkbtjt.html

[S26] C：内存清零
来源：http://hz.jqgfzy.top/gtkuezefvs.html

memset(a, 0, sizeof a);
来源：http://hz.shangyingyoupin.top/gtwmyjrstr.html

[S27] C：定义常量
来源：http://hz.shanyushiyangkeji.top/gtonrijrmh.html

const double PI = 3.14159;
来源：http://hz.svipenyu.cn/gtqajcwdgj.html

[S28] C：静态变量
来源：http://hz.snrcjt.cn/gtyonqdbrg.html

static int counter = 0;
来源：http://hz.yongpay.top/gtmwyuffpk.html

[S29] C：变参函数
来源：http://hz.wangdashe.top/gttopvycvx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.chenlongwang.top/gtzdbwhupt.html

[S30] C：头文件保护
来源：http://hz.yvedp.cn/gtxxjkrhea.html

#ifndef X_H
来源：http://hz.ydjk.org.cn/gtfgouxojg.html

#define X_H
来源：http://hz.hywenlv.cn/gtbapbbbrw.html

#endif
来源：http://hz.xingfuxueyuan.xyz/gtqoxvgkzo.html

[S31] C++：Hello World
来源：http://hz.zhongyouzk.top/gtjewyacvt.html

#include <iostream>
来源：http://hz.jinqigufen.top/gthzghkgvj.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.jinghuilouyu.cn/gtczqesjwm.html

[S32] C++：字符串
来源：http://hz.ppjwa.cn/gtlzipqouy.html

std::string s = "hi";  s += "!";
来源：http://hz.52xcode.cn/gtsaaecymv.html

[S33] C++：vector 增删
来源：http://hz.ybcxt.top/gtxlzahkgs.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.zhiwuduotai.top/gtplbqyceu.html

[S34] C++：遍历 vector
来源：http://hz.zhaomingkeji.xyz/gtzvidngei.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.pycfn.com/gtpgoasqxc.html

[S35] C++：map
来源：http://hz.hnxiangtu.top/gtjbguhplo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.gotoacloud.top/gtljicakwx.html

[S36] C++：unordered_map
来源：http://hz.cdnleiting.top/gtowqicrry.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.feifeiyinyue.top/gtcqpxffjp.html

[S37] C++：set
来源：http://hz.shzxlz.cn/gtvmctgybl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.cashguo.top/gtcmftywdt.html

[S38] C++：排序
来源：http://hz.cqqwz.cn/gtbmplfbtt.html

std::sort(v.begin(), v.end());
来源：http://hz.ppjwa.cn/gtwzihdugz.html

[S39] C++：自定义比较器排序
来源：http://hz.zhiwuduotai.top/gtildhrlnf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.vqdsnc.cn/gtvmswzxnx.html

[S40] C++：查找元素
来源：http://hz.jyoumei.cn/gtrhkcdrqp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.ehwqpu.com/gtlwsyovsk.html

[S41] C++：类与构造函数
来源：http://hz.birdmap.top/gtfjeiergx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.jqgufenzy.top/gtafpmofie.html

[S42] C++：继承与虚函数
来源：http://hz.cucudq.cn/gtwefzdjnp.html

class B : public Base { public: void f() override {} };
来源：http://hz.hnxiangtu.top/gtkfwcbrfa.html

[S43] C++：智能指针
来源：http://hz.redwolf501.top/gtffndvjmq.html

auto p = std::make_unique<int>(5);
来源：http://hz.svipenyu.cn/gtbbvvqarn.html

[S44] C++：引用传参
来源：http://hz.yj20258.top/gtvcnezzbk.html

void inc(int &x) { ++x; }
来源：http://hz.cdnleiting.top/gtxvivcsko.html

[S45] C++：lambda
来源：http://hz.hammf.cn/gtvgupkrrf.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.ybcxt.top/gtplhxwsfr.html

[S46] C++：函数模板
来源：http://hz.gaohongyu789.top/gtbnthlbyg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.wangshuangyany.cn/gtidfcwadh.html

[S47] C++：结构化绑定遍历
来源：http://hz.hfpthk.cn/gtksmypmii.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.haohaochexian.top/gtzcbgizjq.html

[S48] C++：逐行读文件
来源：http://hz.wangdashe.top/gthgffjguk.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jinghuilouyu.cn/gtiwyelipi.html

while (std::getline(in, line)) { }
来源：http://hz.guowangkeji.top/gtvlndzsqw.html

[S49] C++：写文件
来源：http://hz.nanxuanxn.top/gtceztmdlk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.jiagoushi.top/gtfvoyrhpc.html

[S50] C++：格式化数字
来源：http://hz.fzhhl.top/gtwldpvout.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.nwbrower.top/gtwymtgcgn.html

[S51] C++：显式类型转换
来源：http://hz.yanxiufei.cn/gtkrhvzcbd.html

static_cast<double>(a) / b
来源：http://hz.ywan-chungtsiang.top/gtneyehsup.html

[S52] C++：const 与 noexcept
来源：http://hz.shanyushiyangkeji.top/gtftlotaci.html

int size() const noexcept { return n_; }
来源：http://hz.0kj1m.cn/gtrgxffkxt.html

[S53] C++：移动语义
来源：http://hz.hnqzz.top/gtnmgqmghp.html

std::vector<int> w = std::move(v);
来源：http://hz.sweek.top/gtoadshzqb.html

[S54] C++：异常处理
来源：http://hz.wangshuangyany.cn/gtttcxkajz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.snrcjt.cn/gtzavyjzqb.html

[S55] C++：结构化绑定
来源：http://hz.shuidangran.top/gtqxqgmadv.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.yangfankeji.com/gtdqdbjhfc.html

[S56] C++：optional
来源：http://hz.yangfankeji.com/gtcpuxubva.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.zhaomingkeji.xyz/gtiwaybxee.html

[S57] C++：编译期常量
来源：http://hz.wangdashe.top/gtmaezttui.html

constexpr int N = 10;
来源：http://hz.birdmap.top/gteontqtxl.html

[S58] C++：命名空间
来源：http://hz.haohaochexian.top/gtbfeptfio.html

namespace ns { int f() { return 1; } }
来源：http://hz.nwbrower.top/gtariebsli.html

[S59] C++：静态断言
来源：http://hz.zhaomingkeji.xyz/gtlswfoslm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.shzxlz.cn/gtzezblvxf.html

[S60] C++：遍历并删除元素
来源：http://hz.yonumen.top/gttdnxtagd.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.redwolf501.top/gtldksjjkl.html

================================================================================
来源：http://hz.aibaodan.cn/gtsltclvfn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.shanyushiyangkeji.top/gtuvcitkzy.html

================================================================================
来源：http://hz.jlsjyb.cn/gtjxtrwkzx.html

[T01] Kotlin：Hello World
来源：http://hz.jinyuanbaomall.cn/gtkpfaofse.html

println("Hello")
来源：http://hz.ydzc1.top/gtffnrhosy.html

[T02] Kotlin：变量
来源：http://hz.jqgfzy.top/gtfcmneybp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.zhengqikj.top/gtmbkvdigu.html

[T03] Kotlin：字符串模板
来源：http://hz.tian-w.cn/gtyxicrkwv.html

"值: $b"
来源：http://hz.zhiwuduotai.top/gtlmxwzrst.html

[T04] Kotlin：空安全
来源：http://hz.chenjidiqi.icu/gtkeumvzka.html

val n: String? = null;  n?.length
来源：http://hz.quarkkingdee.top/gtzcbnrjqz.html

[T05] Kotlin：when 表达式
来源：http://hz.yongpay.top/gtcuxaszrz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.0kj1m.cn/gtywcvbizf.html

[T06] Kotlin：集合映射
来源：http://hz.pycfn.com/gtydbxyvud.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.fengsongda.top/gtwlnqslpg.html

[T07] Kotlin：集合过滤
来源：http://hz.chenjidiqi.icu/gtvxismxns.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.ydjk.org.cn/gthecsnagv.html

[T08] Kotlin：数据类
来源：http://hz.nwbrower.top/gtoesgyxvu.html

data class User(val name: String, val age: Int)
来源：http://hz.aibaodan.cn/gtterfscsu.html

[T09] Kotlin：扩展函数
来源：http://hz.yvedp.cn/gtlgpsewhx.html

fun String.exclaim() = this + "!"
来源：http://hz.yueranfly.top/gtasnmzqkl.html

[T10] Kotlin：默认参数
来源：http://hz.pengpengdd.cyou/gtxvsrlccu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.xylfe.cn/gtrzvnuvqd.html

[T11] Kotlin：协程
来源：http://hz.zhixingplan.top/gttzmyrung.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.zhaomingkeji.xyz/gtogmozzqt.html

[T12] Kotlin：解构声明
来源：http://hz.hammf.cn/gtdpsanqws.html

val (a, b) = Pair(1, 2)
来源：http://hz.xinyue.icu/gthjxoihpz.html


<!-- 参考信息 -->