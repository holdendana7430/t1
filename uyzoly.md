代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://hz.ywan-chungtsiang.top/gtparryanb.html

[R18] 遍历数组
来源：http://hz.aizwys.cn/gtcgdwcqbo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.52xcode.cn/gtbwyshzyz.html

[R19] 数组长度
来源：http://hz.wangshuangyany.cn/gtrlrfpckh.html

echo "${#arr[@]}"
来源：http://hz.hnqzz.top/gtmfbbnwyk.html

[R20] 关联数组（字典）
来源：http://hz.feifeiyinyue.top/gtxigorltn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.xingfuxueyuan.xyz/gtrzosyrkw.html

[R21] 字符串长度
来源：http://hz.jinyuanbaomall.cn/gtkeltaame.html

echo "${#s}"
来源：http://hz.hnqzz.top/gtolznzvnx.html

[R22] 截取子串
来源：http://hz.zhaomingkeji.xyz/gtfrlflczg.html

echo "${s:0:5}"
来源：http://hz.sysykeji.top/gtujfmcjel.html

[R23] 字符串替换
来源：http://hz.shanyushiyangkeji.top/gtfdvrfijt.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.guowangkeji.top/gtcvrqinsh.html

[R24] 大小写转换
来源：http://hz.daria6918.cn/gtgdxnzzxz.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.hnxiangtu.top/gtjmuifwch.html

[R25] 去后缀 / 去前缀
来源：http://hz.chenlongwang.top/gtykecbgcp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.ivvv.top/gtcztelvhq.html

[R26] 命令替换
来源：http://hz.shzxlz.cn/gtfcnqxnqt.html

now=$(date +%F); echo "$now"
来源：http://hz.cucudq.cn/gtjvrozaeo.html

[R27] 算术展开
来源：http://hz.316326.xyz/gttjorbptz.html

echo $((1 + 2 * 3))
来源：http://hz.sysykeji.top/gtzvbnvpfy.html

[R28] 浮点运算
来源：http://hz.shangyingyoupin.top/gtrekaepyr.html

echo "scale=2; 10/3" | bc
来源：http://hz.xuanzx.com/gtdbhqnhsm.html

[R29] 定义函数
来源：http://hz.yj20258.top/gtvinnlzlr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.zhiwuduotai.top/gttiqwpfpl.html

[R30] 函数返回状态码
来源：http://hz.nwbrower.top/gtoscqilxl.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.snrcjt.cn/gtcgnxovht.html

[R31] 局部变量
来源：http://hz.jinyuanbaomall.cn/gtxecmmyar.html

f() { local x=1; echo "$x"; }
来源：http://hz.gzhubu.top/gtdnhretsz.html

[R32] 参数个数校验
来源：http://hz.yueranfly.top/gtoddrsxcm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.havefunace.top/gtwgrqmgbb.html

[R33] 捕获错误并提示行号
来源：http://hz.hysaishi.cn/gtokunrgwl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jinyuanbaomall.cn/gtvdumvion.html

[R34] 退出时清理
来源：http://hz.tanke756.top/gttzcevibc.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.hammf.cn/gtxgndfsyt.html

[R35] 后台执行并等待
来源：http://hz.fzhhl.top/gtmkixecld.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.bjfxy.top/gtsfxadlac.html

[R36] 并发执行多个任务
来源：http://hz.ydzc1.top/gtxpqymlah.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.smart0.xyz/gtjmadbdji.html

[R37] 把输出赋给变量
来源：http://hz.zhixingplan.top/gtywbnyede.html

files=$(ls -1)
来源：http://hz.sufxvd.cn/gtzdyuhouv.html

[R38] 管道串联
来源：http://hz.hammf.cn/gtvvcewzop.html

cat a.txt | grep -i error | wc -l
来源：http://hz.mhx1999.top/gtbfotrfnk.html

[R39] 重定向标准输出与错误
来源：http://hz.snrcjt.cn/gtxkgkbxsp.html

cmd > out.log 2>&1
来源：http://hz.daxiang520.top/gtcwahnvzt.html

[R40] 追加写日志
来源：http://hz.ydzc1.top/gtpdubcnqe.html

echo "log" >> out.log
来源：http://hz.jqgufenzy.top/gtnkoawbwp.html

[R41] 丢弃输出
来源：http://hz.xuanzx.com/gtvjmonnoa.html

cmd >/dev/null 2>&1
来源：http://hz.jinghuilouyu.cn/gtvrpnvlaj.html

[R42] 输入重定向
来源：http://hz.xingfuxueyuan.xyz/gtksvfanfm.html

wc -l < a.txt
来源：http://hz.birdmap.top/gtigzyomop.html

[R43] 按名字查找文件
来源：http://hz.pycfn.com/gtanmbqocp.html

find . -name "*.log" -type f
来源：http://hz.chenzaomai.com/gthmnimxqm.html

[R44] 按修改时间查找
来源：http://hz.tian-w.cn/gtasgvdmts.html

find . -mtime -7 -type f
来源：http://hz.gzhubu.top/gtbufhdvtr.html

[R45] 批量删除
来源：http://hz.wangdashe.top/gtylzxcphz.html

find . -name "*.tmp" -delete
来源：http://hz.cucudq.cn/gtgsrvlhub.html

[R46] 递归替换文件内容
来源：http://hz.cucudq.cn/gtketdoxos.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zhongyouzk.top/gttkxehjcm.html

[R47] sed 单行替换
来源：http://hz.nanxuanxn.top/gtzoqhhdqf.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.zycfv.cn/gtpegxzkxl.html

[R48] awk 取指定列
来源：http://hz.yongpay.top/gtbardzewa.html

awk '{print $1, $3}' a.txt
来源：http://hz.0kj1m.cn/gtireazdnr.html

[R49] awk 带条件
来源：http://hz.havefunace.top/gtavaaibjs.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.meibo888.top/gtyddnuwrb.html

[R50] awk 求和
来源：http://hz.daria6918.cn/gtnteqnjjx.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.aibaodan.cn/gtcipgfyoi.html

[R51] 排序去重取前几
来源：http://hz.zhengqikj.top/gtopjbvgeu.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.zhongyouzk.top/gtmwcpwacq.html

[R52] 统计行数
来源：http://hz.yj20258.top/gtagwelzbt.html

wc -l a.txt
来源：http://hz.snrcjt.cn/gtbyhcvmug.html

[R53] 查看文件头与实时尾
来源：http://hz.svipenyu.cn/gtjgmzleez.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.fengsongda.top/gtegyolshb.html

[R54] 比较两个文件
来源：http://hz.yj202588.top/gtxdhvhiwm.html

diff a.txt b.txt
来源：http://hz.ehwqpu.com/gtliliqdwk.html

[R55] 压缩与解压
来源：http://hz.gotoacloud.top/gtcbtjrwlh.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zhixingplan.top/gtgsiklfdy.html

[R56] 远程拷贝
来源：http://hz.daria6918.cn/gtqmqybslo.html

scp file user@host:/path/
来源：http://hz.jinqigufen.top/gtdqutjwxt.html

[R57] 远程执行命令
来源：http://hz.tianlin.xyz/gtchtepoez.html

ssh user@host 'uptime'
来源：http://hz.jinyuanbaomall.cn/gthjccjxff.html

[R58] 下载文件
来源：http://hz.nanxuanxn.top/gthsbtxlst.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.zdqjudy.top/gthrpbsxoc.html

[R59] 发 POST JSON
来源：http://hz.shanyushiyangtech.top/gtgvxghuvg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.tian-w.cn/gthqepkmal.html

[R60] 只看 HTTP 状态码
来源：http://hz.sxryk.cn/gtewycrrai.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.52xcode.cn/gtzeplozpd.html

[R61] 磁盘占用
来源：http://hz.shuidangran.top/gtnlomfxug.html

df -h;  du -sh *
来源：http://hz.ehwqpu.com/gthfthzodj.html

[R62] 找最占空间的文件
来源：http://hz.nanxinkj.top/gtfyprlkjy.html

du -ah . | sort -rh | head -10
来源：http://hz.chenzaomai.com/gtayvcforl.html

[R63] 内存与进程
来源：http://hz.52xcode.cn/gtsskmmeun.html

free -h;  ps aux | grep nginx
来源：http://hz.316326.xyz/gtddiafyqg.html

[R64] 结束进程
来源：http://hz.9152youxi.cn/gtadljxwsu.html

kill -9 $(pgrep -f app.py)
来源：http://hz.shzxlz.cn/gtlwlzyzjn.html

[R65] 查看端口占用
来源：http://hz.ehwqpu.com/gtjxsheahq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.cucudq.cn/gteiykpcxm.html

[R66] 定时任务
来源：http://hz.9152youxi.cn/gtpbkipwtd.html

crontab -e;  crontab -l
来源：http://hz.sysykeji.top/gtypqthpfz.html

[R67] 生成随机十六进制串
来源：http://hz.ehwqpu.com/gtdrufdtgj.html

openssl rand -hex 16
来源：http://hz.zhijiandao.cn/gtntgogdqq.html

[R68] 计算文件校验值
来源：http://hz.yuanzhike.top/gthajpmlvq.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.dianchejie.cn/gtuzoqqltc.html

[R69] 生成随机密码
来源：http://hz.chenjidiqi.icu/gtnhdpoyga.html

head -c 16 /dev/urandom | base64
来源：http://hz.xuanzx.com/gtodzduapg.html

[R70] 时间戳与互转
来源：http://hz.wangshuangyany.cn/gtljxrouyx.html

date +%s;  date -d @1700000000
来源：http://hz.birdmap.top/gtpujzcaxo.html

[R71] 日期格式化
来源：http://hz.zhongyouzk.top/gtxvogfkut.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.daxiang520.top/gtpviqbstp.html

[R72] 等待端口就绪
来源：http://hz.hfpthk.cn/gtwpfgtjwb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.yanxiufei.cn/gtrxuevfef.html

[R73] 分割大日志
来源：http://hz.feifeiyinyue.top/gtbvvluhlz.html

split -l 1000 big.log part_
来源：http://hz.birdmap.top/gtjdujftqs.html

[R74] 批量重命名
来源：http://hz.dianchejie.cn/gtcsfofkmx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.ppjwa.cn/gtyipiafae.html

[R75] 导出环境变量
来源：http://hz.jinghuilouyu.cn/gtyflzxcsf.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yj202588.top/gtejjkjoqo.html

[R76] 使用临时文件
来源：http://hz.jianghu66.top/gtqybrcaah.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhijiandao.cn/gtqvyvrvru.html

[R77] 读取用户输入
来源：http://hz.52xcode.cn/gtowmtvukt.html

read -rp "请输入: " ans
来源：http://hz.xziqi.cn/gtnvjfnlfk.html

[R78] 交互式菜单
来源：http://hz.dashuyun.cn/gthougfqku.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.gaohongyu789.top/gtiicwevts.html

[R79] 解析命令行选项
来源：http://hz.cashguo.top/gtstcgbevx.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.dianchejie.cn/gtydbxupxm.html

[R80] 查看脚本执行耗时
来源：http://hz.xinyue.icu/gtfkajajdo.html

time ./run.sh
来源：http://hz.shangyingyoupin.top/gtekeoiczb.html

================================================================================
来源：http://hz.chenlongwang.top/gtsxypykpb.html

S. C / C++ 专题
来源：http://hz.shzxlz.cn/gthrfnkqhp.html

================================================================================
来源：http://hz.guannengcc.top/gtskelhqma.html

[S01] C：Hello World
来源：http://hz.jqgufenzy.top/gtswyhkpqb.html

#include <stdio.h>
来源：http://hz.c1oappe.top/gtteqytweq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yj202588.top/gthexdghqq.html

[S02] C：变量与格式化输出
来源：http://hz.tian-w.cn/gtfnayaahr.html

int a = 10; printf("%d\n", a);
来源：http://hz.hongshengwenyu.top/gtkswswcia.html

[S03] C：读入整数
来源：http://hz.shanyushiyangtech.top/gtwrjkvhtb.html

int x; scanf("%d", &x);
来源：http://hz.jinqigufen.top/gtombkyukn.html

[S04] C：字符串复制
来源：http://hz.birdmap.top/gtiwjxlvco.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.snrcjt.cn/gtupdlleqn.html

[S05] C：字符串长度
来源：http://hz.zhoulong.xyz/gtmbtmrlht.html

strlen(s)
来源：http://hz.316326.xyz/gtuqhynvbr.html

[S06] C：字符串比较
来源：http://hz.iojbl.cn/gtkqedxdjv.html

strcmp(a, b) == 0
来源：http://hz.chenzaomai.com/gtcchqunhi.html

[S07] C：数组遍历求和
来源：http://hz.c1oappe.top/gthvnwnfpq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.nanxuanxn.top/gtiozujhes.html

[S08] C：动态内存分配与释放
来源：http://hz.quarkkingdee.top/gtvahrnbwv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yanxiufei.cn/gtybupijcp.html

[S09] C：结构体定义与初始化
来源：http://hz.zhengqikj.top/gtlqsuvpyq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.xziqi.cn/gtrszkrlxy.html

[S10] C：指针与解引用
来源：http://hz.ywan-chungtsiang.top/gtwikfmpiw.html

int *p = &a;  *p = 5;
来源：http://hz.gogol.net.cn/gtecswrjdm.html

[S11] C：逐行读文件
来源：http://hz.52xcode.cn/gtejdcadlc.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.zhengqikj.top/gtcwrejbhk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.havefunace.top/gtedyanouz.html

fclose(f);
来源：http://hz.wangshuangyany.cn/gtklckvhjx.html

[S12] C：写文件
来源：http://hz.gotoacloud.top/gtrvwkvkwz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.chenzaomai.com/gtxjhfyiek.html

[S13] C：宏定义
来源：http://hz.yj20258888.top/gtloyyckhl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.jinyuanbaomall.cn/gtnomzhlsn.html

[S14] C：枚举
来源：http://hz.gogol.net.cn/gtslexrbde.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.zhaomingkeji.xyz/gtyqvilzhi.html

[S15] C：类型转换
来源：http://hz.jlsjyb.cn/gtffllyocb.html

(double) a / b
来源：http://hz.jinyuanbaomall.cn/gtdylrpjhp.html

[S16] C：位操作置位
来源：http://hz.c1oappe.top/gtwpmkxaaq.html

x |= (1 << 3);
来源：http://hz.shanyushiyangtech.top/gtyxwryozm.html

[S17] C：安全拼接字符串
来源：http://hz.xinyue.icu/gtkfmsfkrj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.xuanzx.com/gtvtyhtwyk.html

[S18] C：命令行参数
来源：http://hz.daria6918.cn/gtblglzyfs.html

int main(int argc, char **argv)
来源：http://hz.tianlin.xyz/gtokykwhwd.html

[S19] C：快速排序
来源：http://hz.gogol.net.cn/gtvybllevg.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.xziqi.cn/gtbscnyekw.html

[S20] C：二分查找
来源：http://hz.316326.xyz/gtgqmawysr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.pengpengdd.cyou/gtautuerjx.html

[S21] C：字符类别判断
来源：http://hz.xziqi.cn/gtjpnbzjcb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.tian-w.cn/gtyapzfnnz.html

[S22] C：字符串转数字
来源：http://hz.jinyuanbaomall.cn/gtjysagrba.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.sysykeji.top/gtlzlaaite.html

[S23] C：随机数
来源：http://hz.fzhhl.top/gtbvjtvwuz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.chenlongwang.top/gtzymmjkvy.html

[S24] C：获取本地时间
来源：http://hz.feifeiyinyue.top/gtesjtawgo.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.sxryk.cn/gtgqdrmreq.html

[S25] C：内存拷贝
来源：http://hz.shzxlz.cn/gtzvplpdpl.html

memcpy(dst, src, n);
来源：http://hz.yongpay.top/gtqkbaldfe.html

[S26] C：内存清零
来源：http://hz.bjfxy.top/gtkvlypjfy.html

memset(a, 0, sizeof a);
来源：http://hz.fzhhl.top/gthjzwxyks.html

[S27] C：定义常量
来源：http://hz.feifeiyinyue.top/gtkpnzkluy.html

const double PI = 3.14159;
来源：http://hz.yj202588.top/gtsiwjnvuc.html

[S28] C：静态变量
来源：http://hz.hnqzz.top/gtdnngpdmd.html

static int counter = 0;
来源：http://hz.0kj1m.cn/gtptetkzlx.html

[S29] C：变参函数
来源：http://hz.quarkkingdee.top/gtxfvecirp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.yueranfly.top/gtgqpjdjtl.html

[S30] C：头文件保护
来源：http://hz.yj20258.top/gtfbjehsgu.html

#ifndef X_H
来源：http://hz.cheryme.top/gtztfkznpm.html

#define X_H
来源：http://hz.andypj.xyz/gteysgvukj.html

#endif
来源：http://hz.gogol.net.cn/gtqhthbkht.html

[S31] C++：Hello World
来源：http://hz.andypj.xyz/gttzjazpoo.html

#include <iostream>
来源：http://hz.shanyushiyangtech.top/gtbcyybkqn.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.kuanghao11.cn/gtwazuigsq.html

[S32] C++：字符串
来源：http://hz.chenlongwang.top/gtbigcxehc.html

std::string s = "hi";  s += "!";
来源：http://hz.hfpthk.cn/gtabtykcdw.html

[S33] C++：vector 增删
来源：http://hz.chenlongwang.top/gtgwoepfcf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.nwbrower.top/gtdeitzfei.html

[S34] C++：遍历 vector
来源：http://hz.andypj.xyz/gtdlbyswdo.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.hammf.cn/gtosaoiycs.html

[S35] C++：map
来源：http://hz.yanxiufei.cn/gtkkydruci.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shzxlz.cn/gtvgvglyfp.html

[S36] C++：unordered_map
来源：http://hz.iojbl.cn/gtjkluyuso.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.wangdashe.top/gtxfzaqyfg.html

[S37] C++：set
来源：http://hz.zhijiandao.cn/gthsngoxfv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.hnxiangtu.top/gtwsorrzwm.html

[S38] C++：排序
来源：http://hz.guowangkeji.top/gthjzddldj.html

std::sort(v.begin(), v.end());
来源：http://hz.c1oappe.top/gtcsayeokc.html

[S39] C++：自定义比较器排序
来源：http://hz.aibaodan.cn/gtjrwuyxwl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.dashuyun.cn/gtaadltdxi.html

[S40] C++：查找元素
来源：http://hz.svipenyu.cn/gttxsooajd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.snrcjt.cn/gtbfhzwuml.html

[S41] C++：类与构造函数
来源：http://hz.yuanzhike.top/gtdrabvtrt.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.zycfv.cn/gtgwcsqoml.html

[S42] C++：继承与虚函数
来源：http://hz.xuetiantiany.cn/gtesmfkosz.html

class B : public Base { public: void f() override {} };
来源：http://hz.daxiang520.top/gtpnkkxdfo.html

[S43] C++：智能指针
来源：http://hz.yvedp.cn/gtpjxhusfr.html

auto p = std::make_unique<int>(5);
来源：http://hz.dianchejie.cn/gtopwpvfiu.html

[S44] C++：引用传参
来源：http://hz.nanxinkj.top/gtmkcxgqjd.html

void inc(int &x) { ++x; }
来源：http://hz.zhengqikj.top/gtwvzaetes.html

[S45] C++：lambda
来源：http://hz.yuanzhike.top/gtqdkxjggk.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.shangyingyoupin.top/gtcfeoorvd.html

[S46] C++：函数模板
来源：http://hz.zhaomingkeji.xyz/gtjqphxxzy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.chenjidiqi.icu/gtcppufnyo.html

[S47] C++：结构化绑定遍历
来源：http://hz.cheryme.top/gttcnqvesr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.quarkkingdee.top/gthbxrgnbc.html

[S48] C++：逐行读文件
来源：http://hz.xuanzx.com/gtxvoswgel.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.aibaodan.cn/gteitadmuc.html

while (std::getline(in, line)) { }
来源：http://hz.yonumen.top/gtzafuffpf.html

[S49] C++：写文件
来源：http://hz.jqgufenzy.top/gtmxfblewt.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.yuanzhike.top/gtifunaipo.html

[S50] C++：格式化数字
来源：http://hz.iojbl.cn/gtwtatecpf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yangfankeji.com/gtuotipoyy.html

[S51] C++：显式类型转换
来源：http://hz.shanyushiyangtech.top/gtavrndsvu.html

static_cast<double>(a) / b
来源：http://hz.jinghuilouyu.cn/gtbahcidde.html

[S52] C++：const 与 noexcept
来源：http://hz.tianlin.xyz/gttlbjnaml.html

int size() const noexcept { return n_; }
来源：http://hz.zhoulong.xyz/gtyliyhgqy.html

[S53] C++：移动语义
来源：http://hz.ydzc1.top/gtvecacjcg.html

std::vector<int> w = std::move(v);
来源：http://hz.gogol.net.cn/gtrbdfscne.html

[S54] C++：异常处理
来源：http://hz.jinqigufen.top/gtxtwpugyl.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.hongshengwenyu.top/gtvpmtgkvi.html

[S55] C++：结构化绑定
来源：http://hz.daxiang520.top/gtchoxcmyp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.tianlin.xyz/gtkcycjscf.html

[S56] C++：optional
来源：http://hz.vqdsnc.cn/gtgqrattka.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.zycfv.cn/gtbegafsoh.html

[S57] C++：编译期常量
来源：http://hz.316326.xyz/gttbvkkhvx.html

constexpr int N = 10;
来源：http://hz.feifeiyinyue.top/gtxtufoteh.html

[S58] C++：命名空间
来源：http://hz.jiagoushi.top/gtnmfjnuul.html

namespace ns { int f() { return 1; } }
来源：http://hz.yanxiufei.cn/gtznqwgntf.html

[S59] C++：静态断言
来源：http://hz.hnqzz.top/gtkpufcknm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.xylfe.cn/gtvowkzzmo.html

[S60] C++：遍历并删除元素
来源：http://hz.jlsjyb.cn/gtrsnemeev.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.zhaomingkeji.xyz/gtgfsmoeuc.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtyrbhcohs.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yanxiufei.cn/gtemvfxzei.html

================================================================================
来源：http://hz.kuanghao11.cn/gtvovyeokj.html

[T01] Kotlin：Hello World
来源：http://hz.ppjwa.cn/gtzyujlbrr.html

println("Hello")
来源：http://hz.jlsjyb.cn/gtexnghzpl.html

[T02] Kotlin：变量
来源：http://hz.sxryk.cn/gtgjurkxvx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.fzhhl.top/gtudtazxsb.html

[T03] Kotlin：字符串模板
来源：http://hz.yongpay.top/gtjhkjlqhi.html

"值: $b"
来源：http://hz.ywan-chungtsiang.top/gtzsocltie.html

[T04] Kotlin：空安全
来源：http://hz.shuidangran.top/gtaafjarkf.html

val n: String? = null;  n?.length
来源：http://hz.sxryk.cn/gtklqznqqv.html

[T05] Kotlin：when 表达式
来源：http://hz.ppjwa.cn/gtgpqchqar.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yvedp.cn/gtxwjvmgpq.html

[T06] Kotlin：集合映射
来源：http://hz.chenzaomai.com/gtkjovhzud.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.chenjidiqi.icu/gtcqvzodya.html

[T07] Kotlin：集合过滤
来源：http://hz.guannengcc.top/gtyhtegltl.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.shanyushiyangtech.top/gtkssjcbzt.html

[T08] Kotlin：数据类
来源：http://hz.yj202588.top/gtsuysfotq.html

data class User(val name: String, val age: Int)
来源：http://hz.haohaochexian.top/gtlwtdiyzc.html

[T09] Kotlin：扩展函数
来源：http://hz.ydzc1.top/gtwmnrlccp.html

fun String.exclaim() = this + "!"
来源：http://hz.nwbrower.top/gtboyzrzoi.html

[T10] Kotlin：默认参数
来源：http://hz.yuxming.cn/gtcqoiqvak.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.xuanzx.com/gtmjuxevrv.html

[T11] Kotlin：协程
来源：http://hz.fengsongda.top/gtetjxrcbz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.haohaochexian.top/gtgxgmajpm.html

[T12] Kotlin：解构声明
来源：http://hz.hongshengwenyu.top/gtixkxarja.html

val (a, b) = Pair(1, 2)
来源：http://hz.9152youxi.cn/gtcxqybglg.html

[T13] Kotlin：只读 Map
来源：http://hz.havefunace.top/gtcpccpvoc.html

val m = mapOf("a" to 1)
来源：http://hz.sxryk.cn/gtopuqgusp.html

[T14] Kotlin：循环
来源：http://hz.pycfn.com/gtuyfhltld.html

for (i in 1..10) println(i)
来源：http://hz.andypj.xyz/gtoyysoqyg.html

[T15] Kotlin：接口
来源：http://hz.nanxuanxn.top/gthiakhozm.html

interface Shape { fun area(): Double }
来源：http://hz.pengpengdd.cyou/gtxmdzqndk.html

[T16] Swift：Hello World
来源：http://hz.yanxiufei.cn/gtljvpqirn.html

print("Hello")
来源：http://hz.hfpthk.cn/gtjjyxorlg.html

[T17] Swift：变量与常量
来源：http://hz.shangyingyoupin.top/gtfknxfdbj.html

var a = 1;  let b = 2
来源：http://hz.9152youxi.cn/gtfgtqlnch.html

[T18] Swift：字符串插值
来源：http://hz.wangshuangyany.cn/gthyxcmeyt.html

"值: \(b)"
来源：http://hz.jqgfzy.top/gtuwuwjilp.html

[T19] Swift：可选绑定
来源：http://hz.meibo888.top/gtmqttnkdw.html

if let n = opt { print(n) }
来源：http://hz.xinyue.icu/gtqykplbje.html

[T20] Swift：数组操作
来源：http://hz.yonumen.top/gtrdbadjzx.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jiagoushi.top/gtcggxsaul.html


<!-- 参考信息 -->