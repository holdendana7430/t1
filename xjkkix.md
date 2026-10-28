代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://hz.vqdsnc.cn/gtzpwbkssf.html

[R18] 遍历数组
来源：http://hz.zhijiandao.cn/gtzxpywpmc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.316326.xyz/gtscoouetx.html

[R19] 数组长度
来源：http://hz.yanxiufei.cn/gtkuiddqur.html

echo "${#arr[@]}"
来源：http://hz.yj20258.top/gtqcxilesm.html

[R20] 关联数组（字典）
来源：http://hz.gzhubu.top/gtqtzjryvf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.ivvv.top/gtinkkuzge.html

[R21] 字符串长度
来源：http://hz.zhixingplan.top/gtsbanfzrj.html

echo "${#s}"
来源：http://hz.shanyushiyangkeji.top/gtxkmlrdpm.html

[R22] 截取子串
来源：http://hz.guowangkeji.top/gthgftztuw.html

echo "${s:0:5}"
来源：http://hz.yangfankeji.com/gtrxyyroqk.html

[R23] 字符串替换
来源：http://hz.yvedp.cn/gtjbgpbmtl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.hfpthk.cn/gtpstovlhc.html

[R24] 大小写转换
来源：http://hz.birdmap.top/gtrjwqsfev.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.daxiang520.top/gttiwszdxv.html

[R25] 去后缀 / 去前缀
来源：http://hz.daxiang520.top/gtnxvvcyau.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.jyoumei.cn/gtzvksbzkz.html

[R26] 命令替换
来源：http://hz.jqgufenzy.top/gtylimntdq.html

now=$(date +%F); echo "$now"
来源：http://hz.jqgufenzy.top/gtlrkhdvul.html

[R27] 算术展开
来源：http://hz.pengpengdd.cyou/gtjxelsqjn.html

echo $((1 + 2 * 3))
来源：http://hz.hammf.cn/gtjzqanvxw.html

[R28] 浮点运算
来源：http://hz.jyoumei.cn/gtgqqiojbt.html

echo "scale=2; 10/3" | bc
来源：http://hz.aibaodan.cn/gtphhrdksb.html

[R29] 定义函数
来源：http://hz.yanxiufei.cn/gtpmwxbwes.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.xinyue.icu/gtvsutyekb.html

[R30] 函数返回状态码
来源：http://hz.nanxuanxn.top/gtinpbhrxq.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.9152youxi.cn/gtxbdjcepz.html

[R31] 局部变量
来源：http://hz.wangdashe.top/gtjawajyyz.html

f() { local x=1; echo "$x"; }
来源：http://hz.ywan-chungtsiang.top/gtrowzoxmk.html

[R32] 参数个数校验
来源：http://hz.jinqigfzy.top/gtmrqxmoua.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.havefunace.top/gtstzrwvzk.html

[R33] 捕获错误并提示行号
来源：http://hz.xinyue.icu/gtlssnfjsp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.havefunace.top/gtsoqkzpdh.html

[R34] 退出时清理
来源：http://hz.ehwqpu.com/gtkrprfgvx.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.bjfxy.top/gtsxeukhjj.html

[R35] 后台执行并等待
来源：http://hz.jinghuilouyu.cn/gtaldmzhzc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.xingfuxueyuan.xyz/gtfjrsjxyc.html

[R36] 并发执行多个任务
来源：http://hz.xuetiantiany.cn/gtcspzvumf.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jinyuanbaomall.cn/gtzawptthb.html

[R37] 把输出赋给变量
来源：http://hz.shzxlz.cn/gtqpqxkwix.html

files=$(ls -1)
来源：http://hz.316326.xyz/gtqtpadpnz.html

[R38] 管道串联
来源：http://hz.birdmap.top/gtfthssxhx.html

cat a.txt | grep -i error | wc -l
来源：http://hz.daria6918.cn/gtyxreucch.html

[R39] 重定向标准输出与错误
来源：http://hz.xylfe.cn/gtwtuodkhp.html

cmd > out.log 2>&1
来源：http://hz.pycfn.com/gtpxujjlzx.html

[R40] 追加写日志
来源：http://hz.ydjk.org.cn/gtgqftlpgv.html

echo "log" >> out.log
来源：http://hz.aizwys.cn/gtkcbqiviy.html

[R41] 丢弃输出
来源：http://hz.havefunace.top/gtbcdswzkc.html

cmd >/dev/null 2>&1
来源：http://hz.havefunace.top/gtsngvgziv.html

[R42] 输入重定向
来源：http://hz.andypj.xyz/gtpegnhzrv.html

wc -l < a.txt
来源：http://hz.nanxuanxn.top/gtskzbqbzl.html

[R43] 按名字查找文件
来源：http://hz.gaohongyu789.top/gttceodsnu.html

find . -name "*.log" -type f
来源：http://hz.feifeiyinyue.top/gtscmvzyze.html

[R44] 按修改时间查找
来源：http://hz.shuidangran.top/gtmkzzusys.html

find . -mtime -7 -type f
来源：http://hz.gzhubu.top/gttidpbwwj.html

[R45] 批量删除
来源：http://hz.hnqzz.top/gtewbdqxkj.html

find . -name "*.tmp" -delete
来源：http://hz.smart0.xyz/gtkwbyibtq.html

[R46] 递归替换文件内容
来源：http://hz.chenjidiqi.icu/gtapblvnve.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jinghuilouyu.cn/gtfjjcfhxf.html

[R47] sed 单行替换
来源：http://hz.yvedp.cn/gtmkqapzrf.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.chenzaomai.com/gtzuxsqfyk.html

[R48] awk 取指定列
来源：http://hz.xingfuxueyuan.xyz/gtvyamyaog.html

awk '{print $1, $3}' a.txt
来源：http://hz.gaohongyu789.top/gtawxwsopq.html

[R49] awk 带条件
来源：http://hz.tian-w.cn/gtydplojve.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.52xcode.cn/gtbxorqpwe.html

[R50] awk 求和
来源：http://hz.redwolf501.top/gtblsahjnz.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.316326.xyz/gtkzuoeieb.html

[R51] 排序去重取前几
来源：http://hz.fzhhl.top/gthkqnwlbq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jqgufenzy.top/gtyuwixnaq.html

[R52] 统计行数
来源：http://hz.sufxvd.cn/gttrxqqpzj.html

wc -l a.txt
来源：http://hz.hysaishi.cn/gtszjiyiox.html

[R53] 查看文件头与实时尾
来源：http://hz.chenlongwang.top/gtejhnnfkn.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.zhaomingkeji.xyz/gtithvpnik.html

[R54] 比较两个文件
来源：http://hz.quarkkingdee.top/gtgrfvhxea.html

diff a.txt b.txt
来源：http://hz.zhixingplan.top/gtkvapsohq.html

[R55] 压缩与解压
来源：http://hz.smart0.xyz/gtdzckdrxt.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.tianlin.xyz/gtpwkfgigf.html

[R56] 远程拷贝
来源：http://hz.ehwqpu.com/gtnigzedys.html

scp file user@host:/path/
来源：http://hz.sweek.top/gtsgiixasm.html

[R57] 远程执行命令
来源：http://hz.sufxvd.cn/gtbrgmbfqg.html

ssh user@host 'uptime'
来源：http://hz.ivvv.top/gteccaessm.html

[R58] 下载文件
来源：http://hz.meibo888.top/gtitvpdway.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jianghu66.top/gtcvejtlzv.html

[R59] 发 POST JSON
来源：http://hz.mhx1999.top/gtuoyxajrk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.nanxinkj.top/gttylxrowl.html

[R60] 只看 HTTP 状态码
来源：http://hz.zdqjudy.top/gtymwunpbu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jinqigufen.top/gtxsdedpyn.html

[R61] 磁盘占用
来源：http://hz.jqgufenzy.top/gtgnhqsgfw.html

df -h;  du -sh *
来源：http://hz.mhx1999.top/gtoyccmiwd.html

[R62] 找最占空间的文件
来源：http://hz.yongpay.top/gtizaznmlf.html

du -ah . | sort -rh | head -10
来源：http://hz.c1oappe.top/gtqigxkhgh.html

[R63] 内存与进程
来源：http://hz.jinqigfzy.top/gtryztaaog.html

free -h;  ps aux | grep nginx
来源：http://hz.cashguo.top/gtxgzetggx.html

[R64] 结束进程
来源：http://hz.shanyushiyangkeji.top/gthvgvybdz.html

kill -9 $(pgrep -f app.py)
来源：http://hz.zhengqikj.top/gtvmqvdgzh.html

[R65] 查看端口占用
来源：http://hz.kuanghao11.cn/gtvjpwhnih.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.wangshuangyany.cn/gtsvovgapm.html

[R66] 定时任务
来源：http://hz.xuetiantiany.cn/gtnxzgacai.html

crontab -e;  crontab -l
来源：http://hz.sxryk.cn/gtqhyjimgq.html

[R67] 生成随机十六进制串
来源：http://hz.chenzaomai.com/gtorkhrioc.html

openssl rand -hex 16
来源：http://hz.jianghu66.top/gtbpoyprvr.html

[R68] 计算文件校验值
来源：http://hz.dashuyun.cn/gtpfxddodr.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.xuanzx.com/gtjqcjceoq.html

[R69] 生成随机密码
来源：http://hz.wangshuangyany.cn/gtlzmfpwbg.html

head -c 16 /dev/urandom | base64
来源：http://hz.jinyuanbaomall.cn/gtkinptnjb.html

[R70] 时间戳与互转
来源：http://hz.pengpengdd.cyou/gtkgkzfcpl.html

date +%s;  date -d @1700000000
来源：http://hz.ydjk.org.cn/gtuadjywzz.html

[R71] 日期格式化
来源：http://hz.haohaochexian.top/gtqwivmzyn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.gotoacloud.top/gtpdjiejop.html

[R72] 等待端口就绪
来源：http://hz.jianghu66.top/gtqsyyqwuu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zdqjudy.top/gthjahrcak.html

[R73] 分割大日志
来源：http://hz.hysaishi.cn/gtbnjhmbhi.html

split -l 1000 big.log part_
来源：http://hz.feifeiyinyue.top/gtbqsmxwzl.html

[R74] 批量重命名
来源：http://hz.jinyuanbaomall.cn/gtiuenklpn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.ehwqpu.com/gtbytxqeor.html

[R75] 导出环境变量
来源：http://hz.tian-w.cn/gtipekugpa.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.cashguo.top/gtbngjyxkk.html

[R76] 使用临时文件
来源：http://hz.nanxuanxn.top/gtcagdttyf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.bjfxy.top/gthadrobyr.html

[R77] 读取用户输入
来源：http://hz.quarkkingdee.top/gtelezunmk.html

read -rp "请输入: " ans
来源：http://hz.gotoacloud.top/gtmppzgeyc.html

[R78] 交互式菜单
来源：http://hz.gogol.net.cn/gtrfpewcjh.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.cheryme.top/gtluhihvfm.html

[R79] 解析命令行选项
来源：http://hz.xziqi.cn/gtlwqlrvto.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.9152youxi.cn/gtetvulayy.html

[R80] 查看脚本执行耗时
来源：http://hz.tian-w.cn/gtojpvzxfl.html

time ./run.sh
来源：http://hz.birdmap.top/gtofopyhyf.html

================================================================================
来源：http://hz.pycfn.com/gtfzmajcrk.html

S. C / C++ 专题
来源：http://hz.9152youxi.cn/gtukxgjlhy.html

================================================================================
来源：http://hz.ydjk.org.cn/gtmccjgtsc.html

[S01] C：Hello World
来源：http://hz.yuxming.cn/gtvvyarafc.html

#include <stdio.h>
来源：http://hz.hywenlv.cn/gtevyfhnhc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.tian-w.cn/gtgvwrzpht.html

[S02] C：变量与格式化输出
来源：http://hz.hywenlv.cn/gtbhctkzrm.html

int a = 10; printf("%d\n", a);
来源：http://hz.xingfuxueyuan.xyz/gtxjnjykfp.html

[S03] C：读入整数
来源：http://hz.kuanghao11.cn/gtpucpvolt.html

int x; scanf("%d", &x);
来源：http://hz.meibo888.top/gtoyfyuinb.html

[S04] C：字符串复制
来源：http://hz.feifeiyinyue.top/gttlkfjddo.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jyoumei.cn/gtjtzhrpuv.html

[S05] C：字符串长度
来源：http://hz.guannengcc.top/gtyfelniil.html

strlen(s)
来源：http://hz.ydzc1.top/gtbbudbigd.html

[S06] C：字符串比较
来源：http://hz.sxryk.cn/gtjjhublng.html

strcmp(a, b) == 0
来源：http://hz.zdqjudy.top/gtvfxilwye.html

[S07] C：数组遍历求和
来源：http://hz.gogol.net.cn/gtinzgokny.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.cucudq.cn/gtapivivgl.html

[S08] C：动态内存分配与释放
来源：http://hz.yonumen.top/gtikkjynqt.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.meibo888.top/gtypdypohv.html

[S09] C：结构体定义与初始化
来源：http://hz.sysykeji.top/gtduclrddo.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.ydjk.org.cn/gtjidliubi.html

[S10] C：指针与解引用
来源：http://hz.chenzaomai.com/gtlznwcred.html

int *p = &a;  *p = 5;
来源：http://hz.dashuyun.cn/gtxliitglp.html

[S11] C：逐行读文件
来源：http://hz.hammf.cn/gtlnmtmlml.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.nanxuanxn.top/gtlzukpfcp.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.fzhhl.top/gtoklfummn.html

fclose(f);
来源：http://hz.zdqjudy.top/gtiilbqrym.html

[S12] C：写文件
来源：http://hz.ywan-chungtsiang.top/gtztbhnfxz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.ydzc1.top/gtjnewrhtc.html

[S13] C：宏定义
来源：http://hz.redwolf501.top/gtgrpninjz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.gogol.net.cn/gtpijiresq.html

[S14] C：枚举
来源：http://hz.yongpay.top/gteikuloyc.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.xuanzx.com/gtykmqokpd.html

[S15] C：类型转换
来源：http://hz.yonumen.top/gttadglult.html

(double) a / b
来源：http://hz.zhoulong.xyz/gtwlytsmer.html

[S16] C：位操作置位
来源：http://hz.hnqzz.top/gtmdwucqoh.html

x |= (1 << 3);
来源：http://hz.xuetiantiany.cn/gtrlffcfvq.html

[S17] C：安全拼接字符串
来源：http://hz.shangyingyoupin.top/gtfzrdshlz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.chenzaomai.com/gtxodkfhhc.html

[S18] C：命令行参数
来源：http://hz.ivvv.top/gtbjvilltt.html

int main(int argc, char **argv)
来源：http://hz.shangyingyoupin.top/gtpdyhocng.html

[S19] C：快速排序
来源：http://hz.xuanzx.com/gthuncflcb.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yvedp.cn/gtpztjctoj.html

[S20] C：二分查找
来源：http://hz.cqqwz.cn/gtaefhwmxi.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.hammf.cn/gtkbmssjge.html

[S21] C：字符类别判断
来源：http://hz.xingfuxueyuan.xyz/gtjhewfrwm.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.xziqi.cn/gtrydyvtow.html

[S22] C：字符串转数字
来源：http://hz.ehwqpu.com/gtmjbjwfcv.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.xinyue.icu/gtbfhgnzuz.html

[S23] C：随机数
来源：http://hz.ywan-chungtsiang.top/gtrxrbwgpv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.vqdsnc.cn/gtxdlscksy.html

[S24] C：获取本地时间
来源：http://hz.andypj.xyz/gttalnhonp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yj20258.top/gtseosbufs.html

[S25] C：内存拷贝
来源：http://hz.yuanzhike.top/gtwsjpidbw.html

memcpy(dst, src, n);
来源：http://hz.yuanzhike.top/gtleuzquuz.html

[S26] C：内存清零
来源：http://hz.svipenyu.cn/gtzgutawso.html

memset(a, 0, sizeof a);
来源：http://hz.gogol.net.cn/gtqnrbfxtw.html

[S27] C：定义常量
来源：http://hz.gotoacloud.top/gtwsgywnjo.html

const double PI = 3.14159;
来源：http://hz.gzhubu.top/gtcwmhveog.html

[S28] C：静态变量
来源：http://hz.zhoulong.xyz/gtuheaimrf.html

static int counter = 0;
来源：http://hz.guowangkeji.top/gtykcnolhn.html

[S29] C：变参函数
来源：http://hz.shanyushiyangtech.top/gtqmugjfki.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zhengqikj.top/gtitgxjnow.html

[S30] C：头文件保护
来源：http://hz.jinyuanbaomall.cn/gterptiwbu.html

#ifndef X_H
来源：http://hz.shuidangran.top/gthdsahkat.html

#define X_H
来源：http://hz.shangyingyoupin.top/gtmheporwo.html

#endif
来源：http://hz.yj202588.top/gtgnjrwhzp.html

[S31] C++：Hello World
来源：http://hz.gotoacloud.top/gtylejglth.html

#include <iostream>
来源：http://hz.yvedp.cn/gtglqslqrm.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.pycfn.com/gtwimnipih.html

[S32] C++：字符串
来源：http://hz.jinyuanbaomall.cn/gtjljkzsyx.html

std::string s = "hi";  s += "!";
来源：http://hz.yuxming.cn/gtphmepzxt.html

[S33] C++：vector 增删
来源：http://hz.fengsongda.top/gtnkskyffh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.xziqi.cn/gtqdcnxvys.html

[S34] C++：遍历 vector
来源：http://hz.bjfxy.top/gtimacqfih.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.andypj.xyz/gtrjaezyln.html

[S35] C++：map
来源：http://hz.havefunace.top/gthauhhqsn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jinghuilouyu.cn/gtbfgntntf.html

[S36] C++：unordered_map
来源：http://hz.cqqwz.cn/gtccadtlrk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.gzhubu.top/gtmpoxqena.html

[S37] C++：set
来源：http://hz.zhengqikj.top/gtrhcpnafu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.pengpengdd.cyou/gtqxkbozzh.html

[S38] C++：排序
来源：http://hz.dashuyun.cn/gtcpqpzcku.html

std::sort(v.begin(), v.end());
来源：http://hz.hywenlv.cn/gtujqjoeru.html

[S39] C++：自定义比较器排序
来源：http://hz.gaohongyu789.top/gtswhuidgp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.fengsongda.top/gtfdolyrse.html

[S40] C++：查找元素
来源：http://hz.hywenlv.cn/gtceymzkwt.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.sufxvd.cn/gtbqdujpsh.html

[S41] C++：类与构造函数
来源：http://hz.chenjidiqi.icu/gtujhevctt.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yangfankeji.com/gtttgoworr.html

[S42] C++：继承与虚函数
来源：http://hz.zhijiandao.cn/gtvyofxnpm.html

class B : public Base { public: void f() override {} };
来源：http://hz.kuanghao11.cn/gtxhxshrbw.html

[S43] C++：智能指针
来源：http://hz.yj202588.top/gtuufzziqj.html

auto p = std::make_unique<int>(5);
来源：http://hz.jlsjyb.cn/gtkqhxrpah.html

[S44] C++：引用传参
来源：http://hz.fengsongda.top/gtdlqxdpqe.html

void inc(int &x) { ++x; }
来源：http://hz.guannengcc.top/gtxjtxpekh.html

[S45] C++：lambda
来源：http://hz.yuanzhike.top/gtzjidqusk.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.yuanzhike.top/gtnkqfxjvp.html

[S46] C++：函数模板
来源：http://hz.gogol.net.cn/gtqhbieihm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.ywan-chungtsiang.top/gtmbmvqfgb.html

[S47] C++：结构化绑定遍历
来源：http://hz.guannengcc.top/gtkabwmokp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.pengpengdd.cyou/gttavwqqtf.html

[S48] C++：逐行读文件
来源：http://hz.yuanzhike.top/gtfjwseofi.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.cheryme.top/gtaytipykh.html

while (std::getline(in, line)) { }
来源：http://hz.xingfuxueyuan.xyz/gtyryhsmpd.html

[S49] C++：写文件
来源：http://hz.jinghuilouyu.cn/gttaujtbkv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.pengpengdd.cyou/gtfvgclvtz.html

[S50] C++：格式化数字
来源：http://hz.yueranfly.top/gtvzsfngzj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.zhongyouzk.top/gtztpljqsm.html

[S51] C++：显式类型转换
来源：http://hz.zdqjudy.top/gtwghombsm.html

static_cast<double>(a) / b
来源：http://hz.guowangkeji.top/gtcagolllk.html

[S52] C++：const 与 noexcept
来源：http://hz.feifeiyinyue.top/gtsvvmbqxc.html

int size() const noexcept { return n_; }
来源：http://hz.yj20258888.top/gtmsqqtwmn.html

[S53] C++：移动语义
来源：http://hz.aibaodan.cn/gthwyrmtuh.html

std::vector<int> w = std::move(v);
来源：http://hz.hnqzz.top/gtlkymgtlz.html

[S54] C++：异常处理
来源：http://hz.ivvv.top/gtxtwxlutp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.cqqwz.cn/gtxbfldfou.html

[S55] C++：结构化绑定
来源：http://hz.jinqigfzy.top/gtadfntimg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.sysykeji.top/gtbvohyikj.html

[S56] C++：optional
来源：http://hz.gzhubu.top/gtpwrtasgx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.xuanzx.com/gtqvnmghls.html

[S57] C++：编译期常量
来源：http://hz.daxiang520.top/gtcuennbbw.html

constexpr int N = 10;
来源：http://hz.smart0.xyz/gtxoftnbef.html

[S58] C++：命名空间
来源：http://hz.xylfe.cn/gtjlcqpawg.html

namespace ns { int f() { return 1; } }
来源：http://hz.yj202588.top/gtlcgvkpmb.html

[S59] C++：静态断言
来源：http://hz.jlsjyb.cn/gtvnlioyes.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.shanyushiyangkeji.top/gtetsgrpaz.html

[S60] C++：遍历并删除元素
来源：http://hz.hysaishi.cn/gtiwrcwsge.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.hysaishi.cn/gthhiaeqjy.html

================================================================================
来源：http://hz.gzhubu.top/gtiydbuhit.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.wangdashe.top/gtypezlkcf.html

================================================================================
来源：http://hz.birdmap.top/gtfwchtryi.html

[T01] Kotlin：Hello World
来源：http://hz.zhixingplan.top/gtoxnuawzy.html

println("Hello")
来源：http://hz.zhoulong.xyz/gtpdjohhsw.html

[T02] Kotlin：变量
来源：http://hz.nwbrower.top/gtmkmtruhr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.sysykeji.top/gtycfabwbq.html

[T03] Kotlin：字符串模板
来源：http://hz.0kj1m.cn/gtwidzzlao.html

"值: $b"
来源：http://hz.shanyushiyangkeji.top/gtstgmcuea.html

[T04] Kotlin：空安全
来源：http://hz.quarkkingdee.top/gtvbwhadfu.html

val n: String? = null;  n?.length
来源：http://hz.andypj.xyz/gtgqwdxbqm.html

[T05] Kotlin：when 表达式
来源：http://hz.bjfxy.top/gtsychddhf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.zhijiandao.cn/gtlllrkxmb.html

[T06] Kotlin：集合映射
来源：http://hz.zhixingplan.top/gttceafmtf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.shuidangran.top/gtjaysyzvr.html

[T07] Kotlin：集合过滤
来源：http://hz.9152youxi.cn/gteeqqxtvu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.zhijiandao.cn/gtkfhwofjp.html

[T08] Kotlin：数据类
来源：http://hz.yongpay.top/gtmwgmicyr.html

data class User(val name: String, val age: Int)
来源：http://hz.quarkkingdee.top/gtiswxkzzr.html

[T09] Kotlin：扩展函数
来源：http://hz.9152youxi.cn/gtjsiqyyun.html

fun String.exclaim() = this + "!"
来源：http://hz.wangshuangyany.cn/gtxprgdawd.html

[T10] Kotlin：默认参数
来源：http://hz.jinqigufen.top/gtvyprmewy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.ywan-chungtsiang.top/gtktmuvlzg.html

[T11] Kotlin：协程
来源：http://hz.birdmap.top/gtafvaxijb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.zycfv.cn/gtbwhyvxpp.html

[T12] Kotlin：解构声明
来源：http://hz.sysykeji.top/gtzdfgfubf.html

val (a, b) = Pair(1, 2)
来源：http://hz.cdnleiting.top/gtxztikvym.html

[T13] Kotlin：只读 Map
来源：http://hz.wangshuangyany.cn/gteculkcgt.html

val m = mapOf("a" to 1)
来源：http://hz.gogol.net.cn/gtylxlhfct.html

[T14] Kotlin：循环
来源：http://hz.guannengcc.top/gtxziemghe.html

for (i in 1..10) println(i)
来源：http://hz.zhijiandao.cn/gtesqsxabs.html

[T15] Kotlin：接口
来源：http://hz.yuanzhike.top/gtmzkyooep.html

interface Shape { fun area(): Double }
来源：http://hz.shanyushiyangkeji.top/gtvomuzgyx.html

[T16] Swift：Hello World
来源：http://hz.shzxlz.cn/gtbfegpjyf.html

print("Hello")
来源：http://hz.ppjwa.cn/gtbwuhtqoj.html

[T17] Swift：变量与常量
来源：http://hz.zhiwuduotai.top/gtjuxcminp.html

var a = 1;  let b = 2
来源：http://hz.gaohongyu789.top/gtbwfijpzy.html

[T18] Swift：字符串插值
来源：http://hz.wangdashe.top/gtkjfxzyjs.html

"值: \(b)"
来源：http://hz.kuanghao11.cn/gtvjyimdlb.html

[T19] Swift：可选绑定
来源：http://hz.cqqwz.cn/gtgopmeepx.html

if let n = opt { print(n) }
来源：http://hz.ybcxt.top/gtmivuscno.html

[T20] Swift：数组操作
来源：http://hz.dianchejie.cn/gtpxechicx.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.aizwys.cn/gtrrplaiyu.html


<!-- 参考信息 -->