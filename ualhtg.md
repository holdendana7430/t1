代发 wailian999

case "$1" in
来源：http://hz.ppjwa.cn/gtnwjwejou.html

start) echo "启动" ;;
来源：http://hz.chenjidiqi.icu/gtxvpqluly.html

stop)  echo "停止" ;;
来源：http://hz.52xcode.cn/gtluysajhs.html

*)     echo "未知命令" ;;
来源：http://hz.quarkkingdee.top/gtjyjfitfd.html

esac
来源：http://hz.zhongyouzk.top/gtoaxsfxdv.html

[R12] for 遍历文件
来源：http://hz.yueranfly.top/gteiowwatf.html

for f in *.txt; do echo "$f"; done
来源：http://hz.zhaomingkeji.xyz/gtxdymvnpf.html

[R13] for 计数循环
来源：http://hz.havefunace.top/gtdjolegwi.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.hfpthk.cn/gtghnhcigt.html

[R14] C 风格 for
来源：http://hz.xylfe.cn/gtpuquipho.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.bjfxy.top/gtgzabyccx.html

[R15] while 逐行读文件
来源：http://hz.smart0.xyz/gtuzifnewe.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.zhoulong.xyz/gtyvvlgsvl.html

[R16] until 等待条件
来源：http://hz.ybcxt.top/gtislrpxwt.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.cheryme.top/gtchihrbbs.html

[R17] 数组定义与取值
来源：http://hz.hnxiangtu.top/gtnbccllrz.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.pycfn.com/gtxmybadbf.html

[R18] 遍历数组
来源：http://hz.cheryme.top/gtmzlflznj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zhiwuduotai.top/gtuxmqnzpp.html

[R19] 数组长度
来源：http://hz.gotoacloud.top/gtzclaawnj.html

echo "${#arr[@]}"
来源：http://hz.ybcxt.top/gtxkrnsghx.html

[R20] 关联数组（字典）
来源：http://hz.wangshuangyany.cn/gtktuvrvid.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.aibaodan.cn/gtoevlyase.html

[R21] 字符串长度
来源：http://hz.ydjk.org.cn/gtddvvzlug.html

echo "${#s}"
来源：http://hz.hysaishi.cn/gtfmgigexw.html

[R22] 截取子串
来源：http://hz.hnqzz.top/gtgoknhjfe.html

echo "${s:0:5}"
来源：http://hz.hnxiangtu.top/gttnvudrgr.html

[R23] 字符串替换
来源：http://hz.jqgfzy.top/gtxnjwlnda.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.cashguo.top/gtwayweqqc.html

[R24] 大小写转换
来源：http://hz.yongpay.top/gttxdihosc.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yj20258.top/gtwwmskdpk.html

[R25] 去后缀 / 去前缀
来源：http://hz.xingfuxueyuan.xyz/gtlskjjsce.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.dianchejie.cn/gtstlazsrg.html

[R26] 命令替换
来源：http://hz.jqgfzy.top/gtqawbampp.html

now=$(date +%F); echo "$now"
来源：http://hz.vqdsnc.cn/gtdscverdi.html

[R27] 算术展开
来源：http://hz.wangshuangyany.cn/gtrstmlwka.html

echo $((1 + 2 * 3))
来源：http://hz.dashuyun.cn/gtcmziiddp.html

[R28] 浮点运算
来源：http://hz.daxiang520.top/gtwiawjeel.html

echo "scale=2; 10/3" | bc
来源：http://hz.52xcode.cn/gtzhmvbuod.html

[R29] 定义函数
来源：http://hz.hywenlv.cn/gtnjgixcpm.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.ydjk.org.cn/gtjjxrjsir.html

[R30] 函数返回状态码
来源：http://hz.pycfn.com/gtfywjxtom.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.svipenyu.cn/gtercuuxlu.html

[R31] 局部变量
来源：http://hz.yuxming.cn/gtbnyywmfx.html

f() { local x=1; echo "$x"; }
来源：http://hz.xinyue.icu/gtrvkbyvsd.html

[R32] 参数个数校验
来源：http://hz.hfpthk.cn/gturzrbwat.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.redwolf501.top/gtgmrknssj.html

[R33] 捕获错误并提示行号
来源：http://hz.fzhhl.top/gtcjbmpsna.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.havefunace.top/gtylznqnhp.html

[R34] 退出时清理
来源：http://hz.sweek.top/gtlimcbuya.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.bjfxy.top/gtxbntmnkc.html

[R35] 后台执行并等待
来源：http://hz.daria6918.cn/gttdegbgau.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jianghu66.top/gtgjyzmhjx.html

[R36] 并发执行多个任务
来源：http://hz.aizwys.cn/gtropmpwju.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.daria6918.cn/gtxdhmdagg.html

[R37] 把输出赋给变量
来源：http://hz.vqdsnc.cn/gtehhbwhjg.html

files=$(ls -1)
来源：http://hz.hfpthk.cn/gtljbcewvb.html

[R38] 管道串联
来源：http://hz.jinqigfzy.top/gtbftkdxzr.html

cat a.txt | grep -i error | wc -l
来源：http://hz.cashguo.top/gtrqknwxql.html

[R39] 重定向标准输出与错误
来源：http://hz.gotoacloud.top/gtrgbcsctz.html

cmd > out.log 2>&1
来源：http://hz.ehwqpu.com/gtrfusljzj.html

[R40] 追加写日志
来源：http://hz.hfpthk.cn/gtibgpebas.html

echo "log" >> out.log
来源：http://hz.ppjwa.cn/gtqsdgojyj.html

[R41] 丢弃输出
来源：http://hz.hnxiangtu.top/gtetzfdbcm.html

cmd >/dev/null 2>&1
来源：http://hz.fzhhl.top/gtmgwbibuy.html

[R42] 输入重定向
来源：http://hz.svipenyu.cn/gtkoisvyoe.html

wc -l < a.txt
来源：http://hz.pengpengdd.cyou/gtfjdlnsgk.html

[R43] 按名字查找文件
来源：http://hz.ydzc1.top/gtfezuavio.html

find . -name "*.log" -type f
来源：http://hz.shuidangran.top/gtcnwqjmdr.html

[R44] 按修改时间查找
来源：http://hz.zhaomingkeji.xyz/gtbcibtgze.html

find . -mtime -7 -type f
来源：http://hz.xingfuxueyuan.xyz/gtcodqeuhv.html

[R45] 批量删除
来源：http://hz.iojbl.cn/gtzrlguxpl.html

find . -name "*.tmp" -delete
来源：http://hz.jyoumei.cn/gtokeqrfuu.html

[R46] 递归替换文件内容
来源：http://hz.iojbl.cn/gtachmzxyx.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yuanzhike.top/gtcxrgxols.html

[R47] sed 单行替换
来源：http://hz.nanxuanxn.top/gtqpmbeyix.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.sysykeji.top/gtvfzsftek.html

[R48] awk 取指定列
来源：http://hz.c1oappe.top/gtcqmhoowf.html

awk '{print $1, $3}' a.txt
来源：http://hz.pengpengdd.cyou/gtfarrcpzz.html

[R49] awk 带条件
来源：http://hz.wangshuangyany.cn/gtjtkkdbmb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.tian-w.cn/gtimfekmte.html

[R50] awk 求和
来源：http://hz.52xcode.cn/gtyexnlwqp.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.shanyushiyangkeji.top/gtzbckdpvl.html

[R51] 排序去重取前几
来源：http://hz.yvedp.cn/gtatnrvmlq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jyoumei.cn/gtasdrzuom.html

[R52] 统计行数
来源：http://hz.jqgfzy.top/gtaxmndihm.html

wc -l a.txt
来源：http://hz.hysaishi.cn/gtnixhnoay.html

[R53] 查看文件头与实时尾
来源：http://hz.yangfankeji.com/gtvfkwchvn.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.snrcjt.cn/gtebmlgyqs.html

[R54] 比较两个文件
来源：http://hz.ybcxt.top/gtvhdvkaqf.html

diff a.txt b.txt
来源：http://hz.gaohongyu789.top/gtqfuqaoap.html

[R55] 压缩与解压
来源：http://hz.ywan-chungtsiang.top/gtyklzrcyt.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zhixingplan.top/gtyghhokdf.html

[R56] 远程拷贝
来源：http://hz.xuanzx.com/gtettifdax.html

scp file user@host:/path/
来源：http://hz.birdmap.top/gtexnwfqvw.html

[R57] 远程执行命令
来源：http://hz.redwolf501.top/gtidzfctbo.html

ssh user@host 'uptime'
来源：http://hz.snrcjt.cn/gtpcenaiqw.html

[R58] 下载文件
来源：http://hz.jiagoushi.top/gtlfzoqphp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.fzhhl.top/gtbnogirzh.html

[R59] 发 POST JSON
来源：http://hz.hongshengwenyu.top/gthbdyaziy.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.daxiang520.top/gtwurmtcuf.html

[R60] 只看 HTTP 状态码
来源：http://hz.iojbl.cn/gtrlpjtktw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.52xcode.cn/gtbazqvodt.html

[R61] 磁盘占用
来源：http://hz.c1oappe.top/gttcrmpwjq.html

df -h;  du -sh *
来源：http://hz.fengsongda.top/gtdrdtrvjw.html

[R62] 找最占空间的文件
来源：http://hz.shzxlz.cn/gtppwnbilf.html

du -ah . | sort -rh | head -10
来源：http://hz.cheryme.top/gtwkorchdf.html

[R63] 内存与进程
来源：http://hz.chenjidiqi.icu/gtfpubavca.html

free -h;  ps aux | grep nginx
来源：http://hz.hywenlv.cn/gtwlafvljs.html

[R64] 结束进程
来源：http://hz.hnqzz.top/gtthefnfup.html

kill -9 $(pgrep -f app.py)
来源：http://hz.hnqzz.top/gtsgyexcch.html

[R65] 查看端口占用
来源：http://hz.chenlongwang.top/gtrpeehzxb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.wangshuangyany.cn/gtlgyzwgvw.html

[R66] 定时任务
来源：http://hz.shuidangran.top/gtalclmdbj.html

crontab -e;  crontab -l
来源：http://hz.gogol.net.cn/gtkgqaibvs.html

[R67] 生成随机十六进制串
来源：http://hz.zhijiandao.cn/gtywahyspw.html

openssl rand -hex 16
来源：http://hz.aizwys.cn/gtrhwpfqdb.html

[R68] 计算文件校验值
来源：http://hz.chenzaomai.com/gthxjvgqoc.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.aibaodan.cn/gtzorlksrq.html

[R69] 生成随机密码
来源：http://hz.vqdsnc.cn/gtxzsgtktl.html

head -c 16 /dev/urandom | base64
来源：http://hz.ehwqpu.com/gtnigxrzjl.html

[R70] 时间戳与互转
来源：http://hz.0kj1m.cn/gtkgczimqx.html

date +%s;  date -d @1700000000
来源：http://hz.sxryk.cn/gtywsmystj.html

[R71] 日期格式化
来源：http://hz.wangshuangyany.cn/gtkunprnth.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.chenzaomai.com/gtadeclklw.html

[R72] 等待端口就绪
来源：http://hz.0kj1m.cn/gtymzvamcl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.wangshuangyany.cn/gtqtfhfreb.html

[R73] 分割大日志
来源：http://hz.zhixingplan.top/gtojkuyzge.html

split -l 1000 big.log part_
来源：http://hz.andypj.xyz/gtdjyarmkw.html

[R74] 批量重命名
来源：http://hz.shangyingyoupin.top/gtaqnixybm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.feifeiyinyue.top/gtdcdvcdod.html

[R75] 导出环境变量
来源：http://hz.yj20258888.top/gtsfclrftg.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.nwbrower.top/gtwmlziwdz.html

[R76] 使用临时文件
来源：http://hz.0kj1m.cn/gtylpvyvau.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.gotoacloud.top/gtsciwetfa.html

[R77] 读取用户输入
来源：http://hz.ehwqpu.com/gtqowwkdxm.html

read -rp "请输入: " ans
来源：http://hz.hnxiangtu.top/gtbefpvysb.html

[R78] 交互式菜单
来源：http://hz.hnxiangtu.top/gtpsbzxpks.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.meibo888.top/gtinvtvntj.html

[R79] 解析命令行选项
来源：http://hz.aibaodan.cn/gtklsvwwcf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.andypj.xyz/gtedcentkw.html

[R80] 查看脚本执行耗时
来源：http://hz.yj20258.top/gtseeonkcg.html

time ./run.sh
来源：http://hz.ydjk.org.cn/gtzouhekmp.html

================================================================================
来源：http://hz.dashuyun.cn/gtkrpqhuzn.html

S. C / C++ 专题
来源：http://hz.gzhubu.top/gtarqonslx.html

================================================================================
来源：http://hz.shzxlz.cn/gtzobnskuf.html

[S01] C：Hello World
来源：http://hz.ydjk.org.cn/gthywhldsq.html

#include <stdio.h>
来源：http://hz.smart0.xyz/gtazawnofz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.zhoulong.xyz/gtgcrdvgos.html

[S02] C：变量与格式化输出
来源：http://hz.zhongyouzk.top/gtorxabhkp.html

int a = 10; printf("%d\n", a);
来源：http://hz.9152youxi.cn/gtunjixzds.html

[S03] C：读入整数
来源：http://hz.xuanzx.com/gtelvffmtd.html

int x; scanf("%d", &x);
来源：http://hz.gzhubu.top/gtnxxsrojf.html

[S04] C：字符串复制
来源：http://hz.gogol.net.cn/gtpipxgsji.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zhiwuduotai.top/gtqdmpwpxc.html

[S05] C：字符串长度
来源：http://hz.ywan-chungtsiang.top/gtnmwsurjh.html

strlen(s)
来源：http://hz.shanyushiyangkeji.top/gtvyzrfrtu.html

[S06] C：字符串比较
来源：http://hz.hnxiangtu.top/gtdxwylxhx.html

strcmp(a, b) == 0
来源：http://hz.jianghu66.top/gtqekhdnyl.html

[S07] C：数组遍历求和
来源：http://hz.aibaodan.cn/gtkhhmnywa.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.hnqzz.top/gtpklsqmao.html

[S08] C：动态内存分配与释放
来源：http://hz.gogol.net.cn/gtantdlbtd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.cheryme.top/gtbxntcisd.html

[S09] C：结构体定义与初始化
来源：http://hz.daria6918.cn/gtzjspvlzc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.jlsjyb.cn/gtpxfftooy.html

[S10] C：指针与解引用
来源：http://hz.wangshuangyany.cn/gtnstfnicp.html

int *p = &a;  *p = 5;
来源：http://hz.ywan-chungtsiang.top/gtjbiesmzk.html

[S11] C：逐行读文件
来源：http://hz.zhoulong.xyz/gtxihaiqim.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.zdqjudy.top/gtzttywtmw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.fzhhl.top/gtfbadmtlv.html

fclose(f);
来源：http://hz.hnxiangtu.top/gtoelcopgm.html

[S12] C：写文件
来源：http://hz.zdqjudy.top/gtibygivtv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.tanke756.top/gtchxwoukc.html

[S13] C：宏定义
来源：http://hz.chenlongwang.top/gtgekcfsxv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.ppjwa.cn/gtgfydmorw.html

[S14] C：枚举
来源：http://hz.chenzaomai.com/gtougeiqvi.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.gzhubu.top/gtrbpibbgy.html

[S15] C：类型转换
来源：http://hz.cashguo.top/gtbcghxejl.html

(double) a / b
来源：http://hz.jqgufenzy.top/gtinkxynjw.html

[S16] C：位操作置位
来源：http://hz.tianlin.xyz/gtthewnuhx.html

x |= (1 << 3);
来源：http://hz.shangyingyoupin.top/gtwwwvnndk.html

[S17] C：安全拼接字符串
来源：http://hz.quarkkingdee.top/gtpllqjtrf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.hysaishi.cn/gtsnibhwvt.html

[S18] C：命令行参数
来源：http://hz.zhijiandao.cn/gtkckkfyju.html

int main(int argc, char **argv)
来源：http://hz.wangshuangyany.cn/gtpqtdqjkg.html

[S19] C：快速排序
来源：http://hz.zhiwuduotai.top/gtffntmbim.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jinyuanbaomall.cn/gtylixmacv.html

[S20] C：二分查找
来源：http://hz.redwolf501.top/gtwdoqwzkc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zhijiandao.cn/gtmpjxqzoa.html

[S21] C：字符类别判断
来源：http://hz.shanyushiyangkeji.top/gtvlfkhphk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jinghuilouyu.cn/gtskkxshsl.html

[S22] C：字符串转数字
来源：http://hz.hnqzz.top/gtmrtkqcvz.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.jyoumei.cn/gtmxsncdqs.html

[S23] C：随机数
来源：http://hz.guowangkeji.top/gttudrzgeh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.ywan-chungtsiang.top/gtsusobunt.html

[S24] C：获取本地时间
来源：http://hz.tianlin.xyz/gtcwvydolf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.haohaochexian.top/gtomupfebm.html

[S25] C：内存拷贝
来源：http://hz.hongshengwenyu.top/gtwwlnjgjb.html

memcpy(dst, src, n);
来源：http://hz.cdnleiting.top/gtfumvnksz.html

[S26] C：内存清零
来源：http://hz.zhengqikj.top/gtbwqziksc.html

memset(a, 0, sizeof a);
来源：http://hz.jinqigfzy.top/gtdfzpvjjg.html

[S27] C：定义常量
来源：http://hz.snrcjt.cn/gtalwzlvtg.html

const double PI = 3.14159;
来源：http://hz.aibaodan.cn/gtlpsevpac.html

[S28] C：静态变量
来源：http://hz.xingfuxueyuan.xyz/gtlyqiqvye.html

static int counter = 0;
来源：http://hz.gaohongyu789.top/gtdfsxyxxx.html

[S29] C：变参函数
来源：http://hz.daxiang520.top/gtmsfytceh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.fengsongda.top/gtvokgmnjg.html

[S30] C：头文件保护
来源：http://hz.jqgufenzy.top/gthatyokje.html

#ifndef X_H
来源：http://hz.wangshuangyany.cn/gtlrulbpza.html

#define X_H
来源：http://hz.zhengqikj.top/gtbtfbtokf.html

#endif
来源：http://hz.ybcxt.top/gtgnpkolbq.html

[S31] C++：Hello World
来源：http://hz.hammf.cn/gtmjezafop.html

#include <iostream>
来源：http://hz.sweek.top/gtxnllldfi.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.wangdashe.top/gtfnvvseea.html

[S32] C++：字符串
来源：http://hz.jinyuanbaomall.cn/gtygsuecsz.html

std::string s = "hi";  s += "!";
来源：http://hz.quarkkingdee.top/gtlhesyphl.html

[S33] C++：vector 增删
来源：http://hz.52xcode.cn/gtgoamuwpo.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.sysykeji.top/gtebbocwdv.html

[S34] C++：遍历 vector
来源：http://hz.hywenlv.cn/gtrunrobrl.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.birdmap.top/gtqcnvpueo.html

[S35] C++：map
来源：http://hz.tian-w.cn/gtzfvpklcz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yj202588.top/gtparfnhfp.html

[S36] C++：unordered_map
来源：http://hz.yueranfly.top/gtfruslcpz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.svipenyu.cn/gtvxoacxpx.html

[S37] C++：set
来源：http://hz.wangdashe.top/gtyfrkdaer.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.zhoulong.xyz/gtufntufzk.html

[S38] C++：排序
来源：http://hz.jyoumei.cn/gtvkjklgkq.html

std::sort(v.begin(), v.end());
来源：http://hz.havefunace.top/gtzmhxonio.html

[S39] C++：自定义比较器排序
来源：http://hz.ehwqpu.com/gtjrtkrmtx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.zdqjudy.top/gtjhuilmba.html

[S40] C++：查找元素
来源：http://hz.shanyushiyangkeji.top/gtcjcgpufn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.andypj.xyz/gtuqvsmlcd.html

[S41] C++：类与构造函数
来源：http://hz.sxryk.cn/gtusvxzpot.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.meibo888.top/gtzdstwvpo.html

[S42] C++：继承与虚函数
来源：http://hz.nanxinkj.top/gtyadxxutk.html

class B : public Base { public: void f() override {} };
来源：http://hz.shanyushiyangtech.top/gtydhzahth.html

[S43] C++：智能指针
来源：http://hz.sweek.top/gtikzkrtjq.html

auto p = std::make_unique<int>(5);
来源：http://hz.c1oappe.top/gtikueowso.html

[S44] C++：引用传参
来源：http://hz.hnxiangtu.top/gtibkjkanv.html

void inc(int &x) { ++x; }
来源：http://hz.andypj.xyz/gtuvrkoing.html

[S45] C++：lambda
来源：http://hz.hongshengwenyu.top/gtbzgcjchh.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.svipenyu.cn/gtjbmpswdi.html

[S46] C++：函数模板
来源：http://hz.ivvv.top/gtqsdnjexb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.snrcjt.cn/gtdjgsycox.html

[S47] C++：结构化绑定遍历
来源：http://hz.yueranfly.top/gtjdfqhshl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.redwolf501.top/gtbmbktfoo.html

[S48] C++：逐行读文件
来源：http://hz.yj20258.top/gtzniphvvu.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.pycfn.com/gtqqrhgnrw.html

while (std::getline(in, line)) { }
来源：http://hz.jlsjyb.cn/gtsknuzqza.html

[S49] C++：写文件
来源：http://hz.nanxuanxn.top/gttjjjcqan.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.jinghuilouyu.cn/gtfyfdtwej.html

[S50] C++：格式化数字
来源：http://hz.fengsongda.top/gtwctymvyn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.fengsongda.top/gtlhxjefwu.html

[S51] C++：显式类型转换
来源：http://hz.tian-w.cn/gtageyqoum.html

static_cast<double>(a) / b
来源：http://hz.shangyingyoupin.top/gtukpuekww.html

[S52] C++：const 与 noexcept
来源：http://hz.hywenlv.cn/gtsznntpeo.html

int size() const noexcept { return n_; }
来源：http://hz.jinyuanbaomall.cn/gtshllyenp.html

[S53] C++：移动语义
来源：http://hz.ywan-chungtsiang.top/gtyqlvopci.html

std::vector<int> w = std::move(v);
来源：http://hz.fengsongda.top/gtrllkghmg.html

[S54] C++：异常处理
来源：http://hz.aibaodan.cn/gtftewrcfm.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.svipenyu.cn/gtyfuhwmxc.html

[S55] C++：结构化绑定
来源：http://hz.cheryme.top/gtqutnaraf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.gzhubu.top/gtekgefoeq.html

[S56] C++：optional
来源：http://hz.0kj1m.cn/gtfsdihtxb.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.nanxinkj.top/gtcdbvtjny.html

[S57] C++：编译期常量
来源：http://hz.9152youxi.cn/gtkgexuadu.html

constexpr int N = 10;
来源：http://hz.zhijiandao.cn/gtnjmuhdcs.html

[S58] C++：命名空间
来源：http://hz.hywenlv.cn/gtounwjjys.html

namespace ns { int f() { return 1; } }
来源：http://hz.cashguo.top/gtzamqglsl.html

[S59] C++：静态断言
来源：http://hz.sysykeji.top/gtkptondfg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.9152youxi.cn/gtpajgpato.html

[S60] C++：遍历并删除元素
来源：http://hz.hysaishi.cn/gtnivaidba.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jiagoushi.top/gtguqefmqn.html

================================================================================
来源：http://hz.shuidangran.top/gtatekutxg.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.daxiang520.top/gtmciaswzw.html

================================================================================
来源：http://hz.nanxinkj.top/gtklroyyat.html

[T01] Kotlin：Hello World
来源：http://hz.gzhubu.top/gtdfojescb.html

println("Hello")
来源：http://hz.meibo888.top/gtuaiuyaoc.html

[T02] Kotlin：变量
来源：http://hz.yanxiufei.cn/gtvxhfxqmj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jinyuanbaomall.cn/gtltyhhgaj.html

[T03] Kotlin：字符串模板
来源：http://hz.cqqwz.cn/gthxwpbpbb.html

"值: $b"
来源：http://hz.zhongyouzk.top/gtgcxlwagn.html

[T04] Kotlin：空安全
来源：http://hz.smart0.xyz/gtgdhjsyvv.html

val n: String? = null;  n?.length
来源：http://hz.jianghu66.top/gtpdkshlsi.html

[T05] Kotlin：when 表达式
来源：http://hz.shanyushiyangtech.top/gtuzavcugu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.wangdashe.top/gtrawfpfml.html

[T06] Kotlin：集合映射
来源：http://hz.jinghuilouyu.cn/gtdlogubbw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.daria6918.cn/gtpkaynuzd.html

[T07] Kotlin：集合过滤
来源：http://hz.smart0.xyz/gtoyletejb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jyoumei.cn/gtjrmscoxj.html

[T08] Kotlin：数据类
来源：http://hz.chenlongwang.top/gtulrwphna.html

data class User(val name: String, val age: Int)
来源：http://hz.shzxlz.cn/gtgpekyszw.html

[T09] Kotlin：扩展函数
来源：http://hz.aibaodan.cn/gtgrpznbzl.html

fun String.exclaim() = this + "!"
来源：http://hz.guannengcc.top/gtetrjhnuh.html

[T10] Kotlin：默认参数
来源：http://hz.jinqigufen.top/gtxyzitaui.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.bjfxy.top/gtaqymypzs.html

[T11] Kotlin：协程
来源：http://hz.xinyue.icu/gtoqteaszh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.hysaishi.cn/gtlpnarhdk.html

[T12] Kotlin：解构声明
来源：http://hz.zhijiandao.cn/gtwlmifsnd.html

val (a, b) = Pair(1, 2)
来源：http://hz.yj202588.top/gtlqxmifhc.html


<!-- 参考信息 -->