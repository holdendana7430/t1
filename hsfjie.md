代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.chenzaomai.com/gtxxouguuw.html

[R16] until 等待条件
来源：http://hz.jqgufenzy.top/gthkgmihxb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jinyuanbaomall.cn/gtnhjntuij.html

[R17] 数组定义与取值
来源：http://hz.yj20258.top/gtopzorxjn.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jinyuanbaomall.cn/gtssqactif.html

[R18] 遍历数组
来源：http://hz.sufxvd.cn/gtzuyljvcx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.yj20258.top/gtyojqepdd.html

[R19] 数组长度
来源：http://hz.cashguo.top/gtwigtsljr.html

echo "${#arr[@]}"
来源：http://hz.shanyushiyangkeji.top/gtlfbfkpfv.html

[R20] 关联数组（字典）
来源：http://hz.chenlongwang.top/gtkncgvxib.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yonumen.top/gtexnnrvaj.html

[R21] 字符串长度
来源：http://hz.ybcxt.top/gtjnzvavbj.html

echo "${#s}"
来源：http://hz.zhijiandao.cn/gtsfhbkbxc.html

[R22] 截取子串
来源：http://hz.shzxlz.cn/gtpqrevokh.html

echo "${s:0:5}"
来源：http://hz.cucudq.cn/gttzeczvmu.html

[R23] 字符串替换
来源：http://hz.316326.xyz/gtnsigkbza.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.xylfe.cn/gtivcwzzgj.html

[R24] 大小写转换
来源：http://hz.ivvv.top/gtxhgotnlz.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.jianghu66.top/gtplecjbky.html

[R25] 去后缀 / 去前缀
来源：http://hz.zycfv.cn/gtiqbympyh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.zhongyouzk.top/gtqbiviwks.html

[R26] 命令替换
来源：http://hz.ivvv.top/gtxpkkkhps.html

now=$(date +%F); echo "$now"
来源：http://hz.chenlongwang.top/gtqfyayzbf.html

[R27] 算术展开
来源：http://hz.52xcode.cn/gtzxrvfrex.html

echo $((1 + 2 * 3))
来源：http://hz.zhoulong.xyz/gtlrtfaaqz.html

[R28] 浮点运算
来源：http://hz.tian-w.cn/gtollgdaem.html

echo "scale=2; 10/3" | bc
来源：http://hz.fzhhl.top/gtppazjbwr.html

[R29] 定义函数
来源：http://hz.zycfv.cn/gtlvlewuhs.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.aizwys.cn/gtybljxzhk.html

[R30] 函数返回状态码
来源：http://hz.havefunace.top/gthvdpidgt.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.316326.xyz/gtvzueaiby.html

[R31] 局部变量
来源：http://hz.aibaodan.cn/gtwbugvawc.html

f() { local x=1; echo "$x"; }
来源：http://hz.ywan-chungtsiang.top/gtonjutciy.html

[R32] 参数个数校验
来源：http://hz.sxryk.cn/gtmsztbmpa.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.gotoacloud.top/gtdqelsixo.html

[R33] 捕获错误并提示行号
来源：http://hz.gaohongyu789.top/gtdswkwcoj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.pengpengdd.cyou/gtviqfnbgp.html

[R34] 退出时清理
来源：http://hz.shanyushiyangtech.top/gtrkpaajki.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.feifeiyinyue.top/gtngsvqlea.html

[R35] 后台执行并等待
来源：http://hz.yuanzhike.top/gtshqxwcaz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.nanxinkj.top/gtkykgykda.html

[R36] 并发执行多个任务
来源：http://hz.cdnleiting.top/gtdkhymppi.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.zhoulong.xyz/gtnbqfackq.html

[R37] 把输出赋给变量
来源：http://hz.zhixingplan.top/gtnxeyqhvn.html

files=$(ls -1)
来源：http://hz.andypj.xyz/gtmggospoe.html

[R38] 管道串联
来源：http://hz.sweek.top/gtnnbwhuui.html

cat a.txt | grep -i error | wc -l
来源：http://hz.hysaishi.cn/gtxelngdvt.html

[R39] 重定向标准输出与错误
来源：http://hz.ivvv.top/gthkvybtxv.html

cmd > out.log 2>&1
来源：http://hz.meibo888.top/gthwfyhukf.html

[R40] 追加写日志
来源：http://hz.pengpengdd.cyou/gtroyrvqri.html

echo "log" >> out.log
来源：http://hz.zhoulong.xyz/gthvasctsl.html

[R41] 丢弃输出
来源：http://hz.hammf.cn/gtkginymzn.html

cmd >/dev/null 2>&1
来源：http://hz.dashuyun.cn/gtpmkwlamb.html

[R42] 输入重定向
来源：http://hz.yangfankeji.com/gtafavcnwd.html

wc -l < a.txt
来源：http://hz.0kj1m.cn/gtniniuexf.html

[R43] 按名字查找文件
来源：http://hz.pycfn.com/gtgpkgqrsl.html

find . -name "*.log" -type f
来源：http://hz.shuidangran.top/gtqgrdivuq.html

[R44] 按修改时间查找
来源：http://hz.feifeiyinyue.top/gtasepeakn.html

find . -mtime -7 -type f
来源：http://hz.52xcode.cn/gtoolhhvju.html

[R45] 批量删除
来源：http://hz.zhengqikj.top/gtfdhiglhf.html

find . -name "*.tmp" -delete
来源：http://hz.zhengqikj.top/gtgeraghtz.html

[R46] 递归替换文件内容
来源：http://hz.ppjwa.cn/gtlwaolicu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.ybcxt.top/gtwtmdmnjy.html

[R47] sed 单行替换
来源：http://hz.zhengqikj.top/gtiwigyslg.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.hammf.cn/gtphdcdqir.html

[R48] awk 取指定列
来源：http://hz.dianchejie.cn/gtfibndida.html

awk '{print $1, $3}' a.txt
来源：http://hz.guannengcc.top/gtyjieranl.html

[R49] awk 带条件
来源：http://hz.wangdashe.top/gtbsfvghua.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.jinghuilouyu.cn/gtqtznchmr.html

[R50] awk 求和
来源：http://hz.dianchejie.cn/gtfxjgidbv.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.zycfv.cn/gtwydiqyiq.html

[R51] 排序去重取前几
来源：http://hz.quarkkingdee.top/gtrerknhcg.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.ydjk.org.cn/gtoslvqpjl.html

[R52] 统计行数
来源：http://hz.jyoumei.cn/gtjbjrcjiw.html

wc -l a.txt
来源：http://hz.chenzaomai.com/gtkujsqimn.html

[R53] 查看文件头与实时尾
来源：http://hz.jqgufenzy.top/gtaejalcss.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.hywenlv.cn/gtgzkrutzb.html

[R54] 比较两个文件
来源：http://hz.sufxvd.cn/gtlqdmtxnt.html

diff a.txt b.txt
来源：http://hz.sxryk.cn/gtegrexklq.html

[R55] 压缩与解压
来源：http://hz.smart0.xyz/gtpxhpusbd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.gzhubu.top/gtrrljwhpj.html

[R56] 远程拷贝
来源：http://hz.c1oappe.top/gtbaknmjhm.html

scp file user@host:/path/
来源：http://hz.sweek.top/gtttmxkuhs.html

[R57] 远程执行命令
来源：http://hz.yj202588.top/gthnugnith.html

ssh user@host 'uptime'
来源：http://hz.bjfxy.top/gtwovnxmol.html

[R58] 下载文件
来源：http://hz.ywan-chungtsiang.top/gtmzemycvl.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jinqigfzy.top/gtxxoaloxp.html

[R59] 发 POST JSON
来源：http://hz.shanyushiyangkeji.top/gtqcruwkkn.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.xingfuxueyuan.xyz/gtqbmhyohx.html

[R60] 只看 HTTP 状态码
来源：http://hz.cheryme.top/gtgrsyczrf.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.iojbl.cn/gtoblhgfyx.html

[R61] 磁盘占用
来源：http://hz.fzhhl.top/gtfxqfsujc.html

df -h;  du -sh *
来源：http://hz.shangyingyoupin.top/gtbypifwum.html

[R62] 找最占空间的文件
来源：http://hz.tian-w.cn/gttswypskd.html

du -ah . | sort -rh | head -10
来源：http://hz.shuidangran.top/gtameahhqp.html

[R63] 内存与进程
来源：http://hz.andypj.xyz/gtnknurvru.html

free -h;  ps aux | grep nginx
来源：http://hz.zhengqikj.top/gtrepecztm.html

[R64] 结束进程
来源：http://hz.chenlongwang.top/gtzdcsnlkj.html

kill -9 $(pgrep -f app.py)
来源：http://hz.52xcode.cn/gtlxpxsqgq.html

[R65] 查看端口占用
来源：http://hz.gotoacloud.top/gtjhnaysyb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.wangdashe.top/gtfvnyeihz.html

[R66] 定时任务
来源：http://hz.c1oappe.top/gtyknoepha.html

crontab -e;  crontab -l
来源：http://hz.tianlin.xyz/gtmtggxqwm.html

[R67] 生成随机十六进制串
来源：http://hz.snrcjt.cn/gtgkjmcthw.html

openssl rand -hex 16
来源：http://hz.redwolf501.top/gttruecmne.html

[R68] 计算文件校验值
来源：http://hz.daxiang520.top/gthiqamopx.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.jinghuilouyu.cn/gterklavpc.html

[R69] 生成随机密码
来源：http://hz.chenjidiqi.icu/gttdutfcsv.html

head -c 16 /dev/urandom | base64
来源：http://hz.tian-w.cn/gtenwjkyjb.html

[R70] 时间戳与互转
来源：http://hz.bjfxy.top/gtrbfaksbp.html

date +%s;  date -d @1700000000
来源：http://hz.hfpthk.cn/gtiqcbpaye.html

[R71] 日期格式化
来源：http://hz.wangshuangyany.cn/gtxnaxskxl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.cucudq.cn/gtqojukyrk.html

[R72] 等待端口就绪
来源：http://hz.sxryk.cn/gtmoxbotgp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.quarkkingdee.top/gtzllylyjj.html

[R73] 分割大日志
来源：http://hz.jinghuilouyu.cn/gthhntnzes.html

split -l 1000 big.log part_
来源：http://hz.yuanzhike.top/gtnpuowrbk.html

[R74] 批量重命名
来源：http://hz.nwbrower.top/gtxsdzjazf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.dashuyun.cn/gtpdevrvwv.html

[R75] 导出环境变量
来源：http://hz.ydjk.org.cn/gtuzgpulrw.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.zhijiandao.cn/gtwbqxjpbq.html

[R76] 使用临时文件
来源：http://hz.nwbrower.top/gtctzduihm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.wangdashe.top/gtitdbrjne.html

[R77] 读取用户输入
来源：http://hz.daxiang520.top/gtomwzbwor.html

read -rp "请输入: " ans
来源：http://hz.aizwys.cn/gtgpodcilg.html

[R78] 交互式菜单
来源：http://hz.zdqjudy.top/gtenbuxuns.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.quarkkingdee.top/gtvqiwvkke.html

[R79] 解析命令行选项
来源：http://hz.jqgufenzy.top/gttqblkgkg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.ppjwa.cn/gtmqqhaozz.html

[R80] 查看脚本执行耗时
来源：http://hz.chenjidiqi.icu/gtkzzbqvdk.html

time ./run.sh
来源：http://hz.tanke756.top/gtlyaqzntk.html

================================================================================
来源：http://hz.bjfxy.top/gtkwbaqkng.html

S. C / C++ 专题
来源：http://hz.kuanghao11.cn/gtlbxbfynh.html

================================================================================
来源：http://hz.nanxuanxn.top/gtyhqiyeta.html

[S01] C：Hello World
来源：http://hz.cashguo.top/gtfxlpouvt.html

#include <stdio.h>
来源：http://hz.aibaodan.cn/gtjvcbugnw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.quarkkingdee.top/gtudjcwemc.html

[S02] C：变量与格式化输出
来源：http://hz.cdnleiting.top/gtpzariphd.html

int a = 10; printf("%d\n", a);
来源：http://hz.hywenlv.cn/gthwiilsxn.html

[S03] C：读入整数
来源：http://hz.ehwqpu.com/gtxpfujxdz.html

int x; scanf("%d", &x);
来源：http://hz.52xcode.cn/gtepzexnau.html

[S04] C：字符串复制
来源：http://hz.hammf.cn/gtgjpaltrv.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.snrcjt.cn/gtoiwdmypc.html

[S05] C：字符串长度
来源：http://hz.hnxiangtu.top/gtkidypvsw.html

strlen(s)
来源：http://hz.pycfn.com/gtqcirkawz.html

[S06] C：字符串比较
来源：http://hz.xylfe.cn/gtrwbwjbpp.html

strcmp(a, b) == 0
来源：http://hz.hysaishi.cn/gtszojqfto.html

[S07] C：数组遍历求和
来源：http://hz.hammf.cn/gtbsgdztmn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.yongpay.top/gtlwqdqpnj.html

[S08] C：动态内存分配与释放
来源：http://hz.hywenlv.cn/gtjasyahaq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.shuidangran.top/gttqzvxksn.html

[S09] C：结构体定义与初始化
来源：http://hz.jiagoushi.top/gtswcylchw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.zycfv.cn/gtggdkasaj.html

[S10] C：指针与解引用
来源：http://hz.yvedp.cn/gtzadueokw.html

int *p = &a;  *p = 5;
来源：http://hz.guowangkeji.top/gtpzectbnr.html

[S11] C：逐行读文件
来源：http://hz.hnxiangtu.top/gtnmiiwyfo.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.mhx1999.top/gtldnjwahu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.dashuyun.cn/gttlpljyiy.html

fclose(f);
来源：http://hz.xuetiantiany.cn/gtnwnhxzoc.html

[S12] C：写文件
来源：http://hz.svipenyu.cn/gtnkgpdckx.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.xinyue.icu/gtiaacpeqh.html

[S13] C：宏定义
来源：http://hz.zdqjudy.top/gtwujuftrh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.zhengqikj.top/gtvyyxgwnl.html

[S14] C：枚举
来源：http://hz.zhaomingkeji.xyz/gtefnmkazq.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.nanxinkj.top/gttjpuipym.html

[S15] C：类型转换
来源：http://hz.haohaochexian.top/gtltcsjtye.html

(double) a / b
来源：http://hz.ppjwa.cn/gtcbveonfq.html

[S16] C：位操作置位
来源：http://hz.wangdashe.top/gtzqtndgbx.html

x |= (1 << 3);
来源：http://hz.yanxiufei.cn/gtkrmccbew.html

[S17] C：安全拼接字符串
来源：http://hz.zycfv.cn/gtpoujretn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.svipenyu.cn/gtamxsyljl.html

[S18] C：命令行参数
来源：http://hz.sxryk.cn/gtbrhvhuza.html

int main(int argc, char **argv)
来源：http://hz.hywenlv.cn/gtzaoufjbt.html

[S19] C：快速排序
来源：http://hz.shuidangran.top/gtqfkncjdi.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.sufxvd.cn/gtdsqelqtl.html

[S20] C：二分查找
来源：http://hz.iojbl.cn/gthbpwwvgs.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.dashuyun.cn/gtjslgmaru.html

[S21] C：字符类别判断
来源：http://hz.gaohongyu789.top/gtqthqysvm.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.ywan-chungtsiang.top/gtdqdogtvm.html

[S22] C：字符串转数字
来源：http://hz.birdmap.top/gtmdstnynx.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yuanzhike.top/gtafpcbbgf.html

[S23] C：随机数
来源：http://hz.guowangkeji.top/gtpyjibery.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.cashguo.top/gtarlqskbr.html

[S24] C：获取本地时间
来源：http://hz.daria6918.cn/gtghpghtkl.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.ywan-chungtsiang.top/gtmmpcacmf.html

[S25] C：内存拷贝
来源：http://hz.jyoumei.cn/gthwoqfmkf.html

memcpy(dst, src, n);
来源：http://hz.yonumen.top/gttytgklwl.html

[S26] C：内存清零
来源：http://hz.hfpthk.cn/gtqajyfazz.html

memset(a, 0, sizeof a);
来源：http://hz.iojbl.cn/gtjmawfvdz.html

[S27] C：定义常量
来源：http://hz.chenzaomai.com/gtjtugmynb.html

const double PI = 3.14159;
来源：http://hz.hfpthk.cn/gtohmfsixo.html

[S28] C：静态变量
来源：http://hz.redwolf501.top/gtvhbxyhsh.html

static int counter = 0;
来源：http://hz.chenlongwang.top/gtzwocgirt.html

[S29] C：变参函数
来源：http://hz.jinghuilouyu.cn/gtiunocpnq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.cheryme.top/gtjqiawkso.html

[S30] C：头文件保护
来源：http://hz.cheryme.top/gtlxwjgabb.html

#ifndef X_H
来源：http://hz.zdqjudy.top/gtbmuycvey.html

#define X_H
来源：http://hz.hfpthk.cn/gtswdsbsvn.html

#endif
来源：http://hz.ywan-chungtsiang.top/gtklbffuut.html

[S31] C++：Hello World
来源：http://hz.sysykeji.top/gthudtfqby.html

#include <iostream>
来源：http://hz.zhongyouzk.top/gtsndqjwjm.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.shanyushiyangtech.top/gtsnfuqqmh.html

[S32] C++：字符串
来源：http://hz.gzhubu.top/gtvlgrkeqc.html

std::string s = "hi";  s += "!";
来源：http://hz.jlsjyb.cn/gtyzugyphs.html

[S33] C++：vector 增删
来源：http://hz.zhaomingkeji.xyz/gtcxingcem.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yuxming.cn/gtshyhagix.html

[S34] C++：遍历 vector
来源：http://hz.hysaishi.cn/gthflombwg.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.cheryme.top/gtzniwcukw.html

[S35] C++：map
来源：http://hz.shangyingyoupin.top/gtnkfmdjif.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ydjk.org.cn/gtqvukjfep.html

[S36] C++：unordered_map
来源：http://hz.kuanghao11.cn/gtnsordpwc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.52xcode.cn/gtagrwajdi.html

[S37] C++：set
来源：http://hz.haohaochexian.top/gtyxotilld.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.cashguo.top/gtugiyxwey.html

[S38] C++：排序
来源：http://hz.yangfankeji.com/gtyrdaolzt.html

std::sort(v.begin(), v.end());
来源：http://hz.bjfxy.top/gttkacpigy.html

[S39] C++：自定义比较器排序
来源：http://hz.hnqzz.top/gtlvkjxjeb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.sufxvd.cn/gtvfvxknci.html

[S40] C++：查找元素
来源：http://hz.ppjwa.cn/gtokluthms.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.nanxuanxn.top/gtzigwnqho.html

[S41] C++：类与构造函数
来源：http://hz.bjfxy.top/gtjxryibke.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.fzhhl.top/gtqbifojqa.html

[S42] C++：继承与虚函数
来源：http://hz.yanxiufei.cn/gtoxzneaie.html

class B : public Base { public: void f() override {} };
来源：http://hz.feifeiyinyue.top/gtrgdtsxto.html

[S43] C++：智能指针
来源：http://hz.guowangkeji.top/gtaeiwiibw.html

auto p = std::make_unique<int>(5);
来源：http://hz.zhixingplan.top/gtvkzqvmtt.html

[S44] C++：引用传参
来源：http://hz.xingfuxueyuan.xyz/gtxmdcoeoy.html

void inc(int &x) { ++x; }
来源：http://hz.zhengqikj.top/gtssnuyipz.html

[S45] C++：lambda
来源：http://hz.redwolf501.top/gtvurhrkoj.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.ywan-chungtsiang.top/gtzgnrxzks.html

[S46] C++：函数模板
来源：http://hz.cqqwz.cn/gtkfxmufzv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.hammf.cn/gtxahavobt.html

[S47] C++：结构化绑定遍历
来源：http://hz.iojbl.cn/gtzunblalw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.yonumen.top/gtmeryvaah.html

[S48] C++：逐行读文件
来源：http://hz.gzhubu.top/gtevuedukw.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.ydzc1.top/gtdlgfahzq.html

while (std::getline(in, line)) { }
来源：http://hz.wangdashe.top/gtjlkjiajr.html

[S49] C++：写文件
来源：http://hz.jiagoushi.top/gtpbbujsxe.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.hfpthk.cn/gtzkninmxc.html

[S50] C++：格式化数字
来源：http://hz.andypj.xyz/gtqoflolew.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.svipenyu.cn/gtqnmogulq.html

[S51] C++：显式类型转换
来源：http://hz.nanxinkj.top/gtguwbaoeh.html

static_cast<double>(a) / b
来源：http://hz.aizwys.cn/gtvonomlnc.html

[S52] C++：const 与 noexcept
来源：http://hz.52xcode.cn/gtykejuatj.html

int size() const noexcept { return n_; }
来源：http://hz.zhijiandao.cn/gtgdpppily.html

[S53] C++：移动语义
来源：http://hz.hysaishi.cn/gtlidfggtq.html

std::vector<int> w = std::move(v);
来源：http://hz.wangshuangyany.cn/gtcxlenagf.html

[S54] C++：异常处理
来源：http://hz.gotoacloud.top/gtugbmxlke.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.hnqzz.top/gtgfehivcn.html

[S55] C++：结构化绑定
来源：http://hz.yvedp.cn/gtvlcqzvfs.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.feifeiyinyue.top/gtafzywzca.html

[S56] C++：optional
来源：http://hz.nanxuanxn.top/gtoliknquy.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.aizwys.cn/gteqgsitdm.html

[S57] C++：编译期常量
来源：http://hz.guowangkeji.top/gtsbyawmcd.html

constexpr int N = 10;
来源：http://hz.tianlin.xyz/gtxzlgxwsr.html

[S58] C++：命名空间
来源：http://hz.pycfn.com/gtnfddhizr.html

namespace ns { int f() { return 1; } }
来源：http://hz.0kj1m.cn/gtsnxdoubo.html

[S59] C++：静态断言
来源：http://hz.cucudq.cn/gtmcybvkvo.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.ybcxt.top/gtlmjtojvx.html

[S60] C++：遍历并删除元素
来源：http://hz.0kj1m.cn/gtwmskaked.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.gotoacloud.top/gthlownoqu.html

================================================================================
来源：http://hz.shzxlz.cn/gttsrvyjlt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.dianchejie.cn/gtdnnnejun.html

================================================================================
来源：http://hz.aizwys.cn/gtctrlrjbm.html

[T01] Kotlin：Hello World
来源：http://hz.zhiwuduotai.top/gtelsmjkbe.html

println("Hello")
来源：http://hz.guannengcc.top/gtasuadfpq.html

[T02] Kotlin：变量
来源：http://hz.xinyue.icu/gtrwurbgdt.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.shzxlz.cn/gtveyrqbut.html

[T03] Kotlin：字符串模板
来源：http://hz.sweek.top/gtbhkumbtw.html

"值: $b"
来源：http://hz.andypj.xyz/gtbspyrxrr.html

[T04] Kotlin：空安全
来源：http://hz.shuidangran.top/gthazvbmbf.html

val n: String? = null;  n?.length
来源：http://hz.andypj.xyz/gtiezwmcuq.html

[T05] Kotlin：when 表达式
来源：http://hz.vqdsnc.cn/gtcqlphgqw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.ehwqpu.com/gtsuigzhlq.html

[T06] Kotlin：集合映射
来源：http://hz.jinghuilouyu.cn/gtcwrivwnf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.aibaodan.cn/gtnbdbbxqe.html

[T07] Kotlin：集合过滤
来源：http://hz.chenlongwang.top/gtxicebjxi.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.hnxiangtu.top/gtugtuneju.html

[T08] Kotlin：数据类
来源：http://hz.tanke756.top/gtctmbgfpj.html

data class User(val name: String, val age: Int)
来源：http://hz.smart0.xyz/gtqryavbgu.html

[T09] Kotlin：扩展函数
来源：http://hz.shangyingyoupin.top/gtdurritgv.html

fun String.exclaim() = this + "!"
来源：http://hz.bjfxy.top/gtcrdroagu.html

[T10] Kotlin：默认参数
来源：http://hz.ybcxt.top/gtgtpvakqf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yuxming.cn/gtcobrgwwm.html

[T11] Kotlin：协程
来源：http://hz.daxiang520.top/gtlaoxycmv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.shanyushiyangkeji.top/gtahbpysgk.html

[T12] Kotlin：解构声明
来源：http://hz.yj202588.top/gtmlbhlaqq.html

val (a, b) = Pair(1, 2)
来源：http://hz.redwolf501.top/gtottupgzv.html

[T13] Kotlin：只读 Map
来源：http://hz.yj20258888.top/gtekytfvyu.html

val m = mapOf("a" to 1)
来源：http://hz.xziqi.cn/gtkwcezowd.html

[T14] Kotlin：循环
来源：http://hz.shanyushiyangkeji.top/gtjwzkpmso.html

for (i in 1..10) println(i)
来源：http://hz.yonumen.top/gtlopyvqpf.html

[T15] Kotlin：接口
来源：http://hz.hfpthk.cn/gtaugexwjn.html

interface Shape { fun area(): Double }
来源：http://hz.quarkkingdee.top/gtgijxacdp.html

[T16] Swift：Hello World
来源：http://hz.sxryk.cn/gtlzcqilqo.html

print("Hello")
来源：http://hz.gotoacloud.top/gtinwhfwoq.html

[T17] Swift：变量与常量
来源：http://hz.vqdsnc.cn/gtbfexxpsg.html

var a = 1;  let b = 2
来源：http://hz.zhongyouzk.top/gtiaynkrte.html

[T18] Swift：字符串插值
来源：http://hz.xingfuxueyuan.xyz/gtezdlrqlt.html

"值: \(b)"
来源：http://hz.316326.xyz/gtwetvxfqr.html


<!-- 参考信息 -->