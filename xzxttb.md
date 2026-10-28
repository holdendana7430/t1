代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.hongshengwenyu.top/gtdfkzbtcu.html

[R16] until 等待条件
来源：http://hz.shanyushiyangtech.top/gteitpqsfd.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.hnxiangtu.top/gtccwvcywz.html

[R17] 数组定义与取值
来源：http://hz.sweek.top/gtqpnkorjx.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.zhiwuduotai.top/gthzlfeqgd.html

[R18] 遍历数组
来源：http://hz.svipenyu.cn/gtcbbqsfsc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.hnqzz.top/gtgndpbobp.html

[R19] 数组长度
来源：http://hz.sxryk.cn/gtcilmxxta.html

echo "${#arr[@]}"
来源：http://hz.hongshengwenyu.top/gtkkgrgges.html

[R20] 关联数组（字典）
来源：http://hz.birdmap.top/gthoksxtmd.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zhoulong.xyz/gtmbcfzjtp.html

[R21] 字符串长度
来源：http://hz.haohaochexian.top/gtkpnbndzn.html

echo "${#s}"
来源：http://hz.hongshengwenyu.top/gteihxlfue.html

[R22] 截取子串
来源：http://hz.havefunace.top/gtufkgtdmb.html

echo "${s:0:5}"
来源：http://hz.xziqi.cn/gttdynqakd.html

[R23] 字符串替换
来源：http://hz.aibaodan.cn/gtfsdqfccl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.fzhhl.top/gtpkntadqx.html

[R24] 大小写转换
来源：http://hz.gaohongyu789.top/gtpunslmya.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.cheryme.top/gtapbqxbxq.html

[R25] 去后缀 / 去前缀
来源：http://hz.zhaomingkeji.xyz/gtoeolrney.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.jyoumei.cn/gtqyoenamm.html

[R26] 命令替换
来源：http://hz.ehwqpu.com/gtfpnzhsam.html

now=$(date +%F); echo "$now"
来源：http://hz.aibaodan.cn/gtcfukmhzy.html

[R27] 算术展开
来源：http://hz.hnxiangtu.top/gtnkttljse.html

echo $((1 + 2 * 3))
来源：http://hz.sufxvd.cn/gtnbsxpbvb.html

[R28] 浮点运算
来源：http://hz.vqdsnc.cn/gtbrlyalpd.html

echo "scale=2; 10/3" | bc
来源：http://hz.ivvv.top/gtvvmqwqev.html

[R29] 定义函数
来源：http://hz.jinghuilouyu.cn/gtjnvjgdov.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jinqigufen.top/gtqrbckrlh.html

[R30] 函数返回状态码
来源：http://hz.iojbl.cn/gteogmimeq.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.hnxiangtu.top/gtuhforzwo.html

[R31] 局部变量
来源：http://hz.andypj.xyz/gtiobrulfe.html

f() { local x=1; echo "$x"; }
来源：http://hz.jinqigufen.top/gtcqfwnwwr.html

[R32] 参数个数校验
来源：http://hz.yj20258888.top/gtxziyupmh.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.9152youxi.cn/gtlbrvupiu.html

[R33] 捕获错误并提示行号
来源：http://hz.fengsongda.top/gtyhulhzvj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.ivvv.top/gtuoziisyp.html

[R34] 退出时清理
来源：http://hz.dianchejie.cn/gtlfxiedcq.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.hnqzz.top/gttktyvvhr.html

[R35] 后台执行并等待
来源：http://hz.xuetiantiany.cn/gtowfkjzyk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jqgufenzy.top/gtosrmeqdq.html

[R36] 并发执行多个任务
来源：http://hz.cashguo.top/gtdwlmqohn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jianghu66.top/gtdhmuipzu.html

[R37] 把输出赋给变量
来源：http://hz.xziqi.cn/gtjltlmvry.html

files=$(ls -1)
来源：http://hz.birdmap.top/gtjolipqqb.html

[R38] 管道串联
来源：http://hz.yangfankeji.com/gtroewwyrq.html

cat a.txt | grep -i error | wc -l
来源：http://hz.tanke756.top/gtlntobqcr.html

[R39] 重定向标准输出与错误
来源：http://hz.cdnleiting.top/gtjwcvwaas.html

cmd > out.log 2>&1
来源：http://hz.ybcxt.top/gtlkruhzab.html

[R40] 追加写日志
来源：http://hz.cheryme.top/gtuyyhcmxx.html

echo "log" >> out.log
来源：http://hz.chenlongwang.top/gtsrmxqtkd.html

[R41] 丢弃输出
来源：http://hz.zhoulong.xyz/gthnporyrn.html

cmd >/dev/null 2>&1
来源：http://hz.hnxiangtu.top/gtguhlbklm.html

[R42] 输入重定向
来源：http://hz.yueranfly.top/gtlprzgudq.html

wc -l < a.txt
来源：http://hz.zhixingplan.top/gtvgrywwbu.html

[R43] 按名字查找文件
来源：http://hz.ydzc1.top/gtcavlnydb.html

find . -name "*.log" -type f
来源：http://hz.0kj1m.cn/gtjiwsyoom.html

[R44] 按修改时间查找
来源：http://hz.hammf.cn/gtiwqxkssr.html

find . -mtime -7 -type f
来源：http://hz.ehwqpu.com/gtyxahwxuj.html

[R45] 批量删除
来源：http://hz.ybcxt.top/gtdfpdmktv.html

find . -name "*.tmp" -delete
来源：http://hz.zhijiandao.cn/gtvceydmzb.html

[R46] 递归替换文件内容
来源：http://hz.pycfn.com/gtrkoeemhy.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.chenzaomai.com/gtlqkxfdeo.html

[R47] sed 单行替换
来源：http://hz.kuanghao11.cn/gtxbxndioi.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.hnqzz.top/gtukdqbunq.html

[R48] awk 取指定列
来源：http://hz.fengsongda.top/gtuzgcxibm.html

awk '{print $1, $3}' a.txt
来源：http://hz.sysykeji.top/gtkhfriumg.html

[R49] awk 带条件
来源：http://hz.yuanzhike.top/gtdcuxilxg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zhengqikj.top/gtkjtuhotj.html

[R50] awk 求和
来源：http://hz.yj202588.top/gtaecslsag.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.kuanghao11.cn/gtejtjzmia.html

[R51] 排序去重取前几
来源：http://hz.tianlin.xyz/gtrmifqfzm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.sysykeji.top/gtvybcoexz.html

[R52] 统计行数
来源：http://hz.ehwqpu.com/gttbnspdjt.html

wc -l a.txt
来源：http://hz.aibaodan.cn/gtdyqnjhnr.html

[R53] 查看文件头与实时尾
来源：http://hz.yj202588.top/gtvlzewwku.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yonumen.top/gttavpdhmz.html

[R54] 比较两个文件
来源：http://hz.fengsongda.top/gtgwdxtdnk.html

diff a.txt b.txt
来源：http://hz.52xcode.cn/gtbohsmura.html

[R55] 压缩与解压
来源：http://hz.cqqwz.cn/gthwhnfene.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.ppjwa.cn/gtdrznlccv.html

[R56] 远程拷贝
来源：http://hz.sufxvd.cn/gtjeyuimun.html

scp file user@host:/path/
来源：http://hz.c1oappe.top/gtgzfnrzxg.html

[R57] 远程执行命令
来源：http://hz.ydjk.org.cn/gtxuhiquts.html

ssh user@host 'uptime'
来源：http://hz.tian-w.cn/gtwwwuaqge.html

[R58] 下载文件
来源：http://hz.jiagoushi.top/gtrhjlzntr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.zhongyouzk.top/gthddeoijo.html

[R59] 发 POST JSON
来源：http://hz.gzhubu.top/gtbfhxqzfx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.birdmap.top/gtbszwsbcw.html

[R60] 只看 HTTP 状态码
来源：http://hz.cdnleiting.top/gtqtrgmzif.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.yanxiufei.cn/gtukcvnulc.html

[R61] 磁盘占用
来源：http://hz.shangyingyoupin.top/gtmgulaidc.html

df -h;  du -sh *
来源：http://hz.yanxiufei.cn/gthduvdhuu.html

[R62] 找最占空间的文件
来源：http://hz.ydzc1.top/gtjtmpmtcx.html

du -ah . | sort -rh | head -10
来源：http://hz.chenlongwang.top/gtvamfytmt.html

[R63] 内存与进程
来源：http://hz.xinyue.icu/gtnmqxcnog.html

free -h;  ps aux | grep nginx
来源：http://hz.0kj1m.cn/gtfvrlwhve.html

[R64] 结束进程
来源：http://hz.jinqigfzy.top/gtdbfkaiau.html

kill -9 $(pgrep -f app.py)
来源：http://hz.9152youxi.cn/gtmoywrteh.html

[R65] 查看端口占用
来源：http://hz.gogol.net.cn/gtoravftgy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.feifeiyinyue.top/gtfurkqepw.html

[R66] 定时任务
来源：http://hz.316326.xyz/gtducrxqcu.html

crontab -e;  crontab -l
来源：http://hz.yj20258888.top/gtwguqxals.html

[R67] 生成随机十六进制串
来源：http://hz.iojbl.cn/gtywnirxac.html

openssl rand -hex 16
来源：http://hz.c1oappe.top/gtvwfcukid.html

[R68] 计算文件校验值
来源：http://hz.aibaodan.cn/gtblcjgreu.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.hywenlv.cn/gtzzfkcnjh.html

[R69] 生成随机密码
来源：http://hz.gaohongyu789.top/gtehzmlltk.html

head -c 16 /dev/urandom | base64
来源：http://hz.sysykeji.top/gtpnafzuqx.html

[R70] 时间戳与互转
来源：http://hz.sweek.top/gtsthvyokg.html

date +%s;  date -d @1700000000
来源：http://hz.nanxinkj.top/gtmtyngwoy.html

[R71] 日期格式化
来源：http://hz.xziqi.cn/gtebwrlwag.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.0kj1m.cn/gtyxlgqvrf.html

[R72] 等待端口就绪
来源：http://hz.xuetiantiany.cn/gtptfavoye.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.kuanghao11.cn/gtbmtfvrny.html

[R73] 分割大日志
来源：http://hz.guannengcc.top/gtghbimdpe.html

split -l 1000 big.log part_
来源：http://hz.sxryk.cn/gttxphgkyu.html

[R74] 批量重命名
来源：http://hz.shanyushiyangtech.top/gtwuvgxlpz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.0kj1m.cn/gtgruobufm.html

[R75] 导出环境变量
来源：http://hz.cheryme.top/gtmwmqbfjc.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yangfankeji.com/gtthcfqenx.html

[R76] 使用临时文件
来源：http://hz.ehwqpu.com/gtbxuknwcu.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.xinyue.icu/gtpgxhiedp.html

[R77] 读取用户输入
来源：http://hz.yanxiufei.cn/gtqoetrxfc.html

read -rp "请输入: " ans
来源：http://hz.zhiwuduotai.top/gtcemaemml.html

[R78] 交互式菜单
来源：http://hz.jinyuanbaomall.cn/gtakpglqlj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.jyoumei.cn/gtmjildnom.html

[R79] 解析命令行选项
来源：http://hz.hysaishi.cn/gtcxfkfwrm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.feifeiyinyue.top/gtmfzvizog.html

[R80] 查看脚本执行耗时
来源：http://hz.zhiwuduotai.top/gtzjnazqks.html

time ./run.sh
来源：http://hz.gzhubu.top/gtikokaqba.html

================================================================================
来源：http://hz.andypj.xyz/gtwjosnijr.html

S. C / C++ 专题
来源：http://hz.xuanzx.com/gtwfqvfjyh.html

================================================================================
来源：http://hz.bjfxy.top/gtbigwjdvh.html

[S01] C：Hello World
来源：http://hz.guowangkeji.top/gtxdkxgnyo.html

#include <stdio.h>
来源：http://hz.tianlin.xyz/gtjfoputqd.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yongpay.top/gtalhhojlz.html

[S02] C：变量与格式化输出
来源：http://hz.ydzc1.top/gthvwxdkfm.html

int a = 10; printf("%d\n", a);
来源：http://hz.ywan-chungtsiang.top/gthdwhbcjl.html

[S03] C：读入整数
来源：http://hz.yj202588.top/gtymudkrwo.html

int x; scanf("%d", &x);
来源：http://hz.shanyushiyangtech.top/gtwqjppojb.html

[S04] C：字符串复制
来源：http://hz.xylfe.cn/gtkjxbezev.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.ivvv.top/gtgkcpmkek.html

[S05] C：字符串长度
来源：http://hz.shanyushiyangtech.top/gtkmklnygk.html

strlen(s)
来源：http://hz.bjfxy.top/gtuodvfgmo.html

[S06] C：字符串比较
来源：http://hz.gaohongyu789.top/gtmnwaclhq.html

strcmp(a, b) == 0
来源：http://hz.shanyushiyangtech.top/gtzvhtyvtr.html

[S07] C：数组遍历求和
来源：http://hz.chenzaomai.com/gtmlnjiaqd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.zhixingplan.top/gtlwhqbthy.html

[S08] C：动态内存分配与释放
来源：http://hz.ydjk.org.cn/gtsjqbpozr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.mhx1999.top/gtgcuvqamr.html

[S09] C：结构体定义与初始化
来源：http://hz.zhiwuduotai.top/gtrylfrmrx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.snrcjt.cn/gthgwwrbpa.html

[S10] C：指针与解引用
来源：http://hz.dianchejie.cn/gtryiiiacy.html

int *p = &a;  *p = 5;
来源：http://hz.tian-w.cn/gtfwwjmcpu.html

[S11] C：逐行读文件
来源：http://hz.redwolf501.top/gtsizmhoeo.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.zhiwuduotai.top/gtemisklfb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yvedp.cn/gtbxtdowbd.html

fclose(f);
来源：http://hz.birdmap.top/gtihtqzmde.html

[S12] C：写文件
来源：http://hz.yuxming.cn/gtbzhwgbzn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.nanxinkj.top/gtgzlpodjr.html

[S13] C：宏定义
来源：http://hz.snrcjt.cn/gtlxiruhsa.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.jqgfzy.top/gthpxxinfh.html

[S14] C：枚举
来源：http://hz.hywenlv.cn/gtcubmnbbi.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.guowangkeji.top/gtjraymwpq.html

[S15] C：类型转换
来源：http://hz.cheryme.top/gtzocmqxrb.html

(double) a / b
来源：http://hz.zycfv.cn/gtrsvzizgq.html

[S16] C：位操作置位
来源：http://hz.smart0.xyz/gtwpjqhvtp.html

x |= (1 << 3);
来源：http://hz.shanyushiyangkeji.top/gtapiurehj.html

[S17] C：安全拼接字符串
来源：http://hz.hongshengwenyu.top/gtuwacptmz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.feifeiyinyue.top/gttzdjkgbi.html

[S18] C：命令行参数
来源：http://hz.jinqigfzy.top/gtyactjxcd.html

int main(int argc, char **argv)
来源：http://hz.xuetiantiany.cn/gtjkguwtkw.html

[S19] C：快速排序
来源：http://hz.guowangkeji.top/gtcwohpamn.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.haohaochexian.top/gtnzgswolu.html

[S20] C：二分查找
来源：http://hz.vqdsnc.cn/gtcmygfejq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.smart0.xyz/gtftkatrmc.html

[S21] C：字符类别判断
来源：http://hz.quarkkingdee.top/gtgsujowkn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.smart0.xyz/gtxmmzaucd.html

[S22] C：字符串转数字
来源：http://hz.yj202588.top/gtvuqhmxng.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yj202588.top/gtrxwzwhyc.html

[S23] C：随机数
来源：http://hz.bjfxy.top/gtpdhsxdtu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.gotoacloud.top/gtjvnqxsla.html

[S24] C：获取本地时间
来源：http://hz.shangyingyoupin.top/gtmuhgyltl.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.zhongyouzk.top/gtdxzoovcc.html

[S25] C：内存拷贝
来源：http://hz.0kj1m.cn/gtywovapbh.html

memcpy(dst, src, n);
来源：http://hz.jqgufenzy.top/gtzinjnntw.html

[S26] C：内存清零
来源：http://hz.jinqigufen.top/gtoqgtzdgk.html

memset(a, 0, sizeof a);
来源：http://hz.hfpthk.cn/gthjljdlyd.html

[S27] C：定义常量
来源：http://hz.cheryme.top/gtbufcamkn.html

const double PI = 3.14159;
来源：http://hz.hnxiangtu.top/gtkiykuqda.html

[S28] C：静态变量
来源：http://hz.mhx1999.top/gtwpaoxkyk.html

static int counter = 0;
来源：http://hz.shangyingyoupin.top/gtxkxoreix.html

[S29] C：变参函数
来源：http://hz.xylfe.cn/gtrhrqpiwm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.sysykeji.top/gtlhtlmxnl.html

[S30] C：头文件保护
来源：http://hz.jinqigufen.top/gtnplfkhuf.html

#ifndef X_H
来源：http://hz.sysykeji.top/gtnprnbjaj.html

#define X_H
来源：http://hz.hongshengwenyu.top/gtwfpwvicr.html

#endif
来源：http://hz.ivvv.top/gtwspjkzsr.html

[S31] C++：Hello World
来源：http://hz.cashguo.top/gtoeymygmr.html

#include <iostream>
来源：http://hz.sysykeji.top/gtxutqcjow.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.cdnleiting.top/gtroerrxgv.html

[S32] C++：字符串
来源：http://hz.jianghu66.top/gtruoddvix.html

std::string s = "hi";  s += "!";
来源：http://hz.mhx1999.top/gtpepajbei.html

[S33] C++：vector 增删
来源：http://hz.hammf.cn/gtvfbaqhun.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.nanxuanxn.top/gtnpvpizvq.html

[S34] C++：遍历 vector
来源：http://hz.shanyushiyangtech.top/gtubulhbdz.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.xingfuxueyuan.xyz/gtzaxccnrt.html

[S35] C++：map
来源：http://hz.daxiang520.top/gtiutedpsn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yj20258.top/gtsgjtqksj.html

[S36] C++：unordered_map
来源：http://hz.guannengcc.top/gtqvyrwivc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jinqigufen.top/gtxhatxngt.html

[S37] C++：set
来源：http://hz.cdnleiting.top/gtcnzyyyuo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.zdqjudy.top/gtoxpdlmrl.html

[S38] C++：排序
来源：http://hz.tianlin.xyz/gtffydkeem.html

std::sort(v.begin(), v.end());
来源：http://hz.tanke756.top/gtpdnmfqoc.html

[S39] C++：自定义比较器排序
来源：http://hz.zhengqikj.top/gtigcpmjdp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.zhengqikj.top/gtvminxeey.html

[S40] C++：查找元素
来源：http://hz.sxryk.cn/gtrfnowdsy.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.ehwqpu.com/gttyvdjqjz.html

[S41] C++：类与构造函数
来源：http://hz.ybcxt.top/gtvrtwcokf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.zhijiandao.cn/gtrrvuylko.html

[S42] C++：继承与虚函数
来源：http://hz.cqqwz.cn/gtythvhetd.html

class B : public Base { public: void f() override {} };
来源：http://hz.chenlongwang.top/gtynoswyjp.html

[S43] C++：智能指针
来源：http://hz.jyoumei.cn/gtkmrkerhg.html

auto p = std::make_unique<int>(5);
来源：http://hz.ydjk.org.cn/gtoaidgkwz.html

[S44] C++：引用传参
来源：http://hz.shuidangran.top/gtetjlmrer.html

void inc(int &x) { ++x; }
来源：http://hz.jinghuilouyu.cn/gttkqjjhcb.html

[S45] C++：lambda
来源：http://hz.ybcxt.top/gtxwykovua.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jinghuilouyu.cn/gtaaxgnran.html

[S46] C++：函数模板
来源：http://hz.xziqi.cn/gtfpqsssvm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.gaohongyu789.top/gtrzdldsbf.html

[S47] C++：结构化绑定遍历
来源：http://hz.hnqzz.top/gtvfqybldw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.tian-w.cn/gtiszifnfo.html

[S48] C++：逐行读文件
来源：http://hz.nanxinkj.top/gtgnzrwbti.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yongpay.top/gthkphwoqd.html

while (std::getline(in, line)) { }
来源：http://hz.havefunace.top/gteijfcbny.html

[S49] C++：写文件
来源：http://hz.ywan-chungtsiang.top/gtksuwfssj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.dianchejie.cn/gtwhcsrpwn.html

[S50] C++：格式化数字
来源：http://hz.gaohongyu789.top/gtaqrbqatv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.shanyushiyangtech.top/gtgkjnbjxy.html

[S51] C++：显式类型转换
来源：http://hz.nwbrower.top/gtmmlmznvq.html

static_cast<double>(a) / b
来源：http://hz.ydjk.org.cn/gtvqfozkos.html

[S52] C++：const 与 noexcept
来源：http://hz.meibo888.top/gtdhukxjhp.html

int size() const noexcept { return n_; }
来源：http://hz.yueranfly.top/gtfgikbvmi.html

[S53] C++：移动语义
来源：http://hz.shangyingyoupin.top/gtgeeptdsv.html

std::vector<int> w = std::move(v);
来源：http://hz.mhx1999.top/gtcogmljts.html

[S54] C++：异常处理
来源：http://hz.yongpay.top/gtvumjgfyp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.bjfxy.top/gtrnxdubti.html

[S55] C++：结构化绑定
来源：http://hz.cashguo.top/gtoamzvcvw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.dashuyun.cn/gtggncgofm.html

[S56] C++：optional
来源：http://hz.cashguo.top/gtyqwjpfuf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.zdqjudy.top/gtimddzxiz.html

[S57] C++：编译期常量
来源：http://hz.dashuyun.cn/gtprbvgvau.html

constexpr int N = 10;
来源：http://hz.meibo888.top/gtcrzpekqr.html

[S58] C++：命名空间
来源：http://hz.hywenlv.cn/gtyrdaxsfq.html

namespace ns { int f() { return 1; } }
来源：http://hz.redwolf501.top/gtsvelrmwr.html

[S59] C++：静态断言
来源：http://hz.chenzaomai.com/gtexzaywvn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.yj20258888.top/gtgfmvujkh.html

[S60] C++：遍历并删除元素
来源：http://hz.jinqigufen.top/gtfnxzgngu.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.kuanghao11.cn/gtfcsaxmpz.html

================================================================================
来源：http://hz.yj20258.top/gthyladagu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.nanxinkj.top/gtbpwmnrnk.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtnylosdka.html

[T01] Kotlin：Hello World
来源：http://hz.sufxvd.cn/gtbnpvundl.html

println("Hello")
来源：http://hz.bjfxy.top/gtptgpwcwa.html

[T02] Kotlin：变量
来源：http://hz.hnqzz.top/gtkgiofkof.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.xylfe.cn/gttygqxzas.html

[T03] Kotlin：字符串模板
来源：http://hz.sufxvd.cn/gtghhylmgk.html

"值: $b"
来源：http://hz.shangyingyoupin.top/gtibsnkhhq.html

[T04] Kotlin：空安全
来源：http://hz.jinyuanbaomall.cn/gtaxbjbojx.html

val n: String? = null;  n?.length
来源：http://hz.sxryk.cn/gtzwejsadn.html

[T05] Kotlin：when 表达式
来源：http://hz.sweek.top/gtuphqgumi.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.shuidangran.top/gtunajwzzu.html

[T06] Kotlin：集合映射
来源：http://hz.shanyushiyangtech.top/gtijabtkmu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.gzhubu.top/gtmjhdyzky.html

[T07] Kotlin：集合过滤
来源：http://hz.zhixingplan.top/gteiyzqcfw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jinghuilouyu.cn/gtgcqgehgq.html

[T08] Kotlin：数据类
来源：http://hz.jianghu66.top/gtiosuvenl.html

data class User(val name: String, val age: Int)
来源：http://hz.andypj.xyz/gtmuwakuuc.html

[T09] Kotlin：扩展函数
来源：http://hz.jyoumei.cn/gtnlnvxfky.html

fun String.exclaim() = this + "!"
来源：http://hz.xuetiantiany.cn/gttxurxcbm.html

[T10] Kotlin：默认参数
来源：http://hz.sufxvd.cn/gtwzxhfnlj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.316326.xyz/gtznynhetf.html

[T11] Kotlin：协程
来源：http://hz.yvedp.cn/gtctfffpvj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.c1oappe.top/gtqxqzzuzs.html

[T12] Kotlin：解构声明
来源：http://hz.daxiang520.top/gtlcmbcmwq.html

val (a, b) = Pair(1, 2)
来源：http://hz.sufxvd.cn/gtxrrgmuoj.html

[T13] Kotlin：只读 Map
来源：http://hz.shangyingyoupin.top/gtnsxqbdfy.html

val m = mapOf("a" to 1)
来源：http://hz.bjfxy.top/gtpftohfgy.html

[T14] Kotlin：循环
来源：http://hz.0kj1m.cn/gtsvjmzxld.html

for (i in 1..10) println(i)
来源：http://hz.ppjwa.cn/gtgpyvnyni.html

[T15] Kotlin：接口
来源：http://hz.nanxuanxn.top/gtlgrvlckk.html

interface Shape { fun area(): Double }
来源：http://hz.fzhhl.top/gtumpluccy.html

[T16] Swift：Hello World
来源：http://hz.chenzaomai.com/gtzqyrdzoo.html

print("Hello")
来源：http://hz.svipenyu.cn/gtrzwrtbji.html

[T17] Swift：变量与常量
来源：http://hz.sysykeji.top/gtompbuzpz.html

var a = 1;  let b = 2
来源：http://hz.hongshengwenyu.top/gtctsxivtn.html

[T18] Swift：字符串插值
来源：http://hz.aizwys.cn/gtlovlovrr.html

"值: \(b)"
来源：http://hz.yongpay.top/gtncngtmeb.html


<!-- 参考信息 -->