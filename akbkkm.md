代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://hz.9152youxi.cn/gtndlhnoxy.html

[R14] C 风格 for
来源：http://hz.yj20258888.top/gtfhokixfb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.guannengcc.top/gtjecbwvwy.html

[R15] while 逐行读文件
来源：http://hz.ydjk.org.cn/gtgauystnc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.snrcjt.cn/gtvpjzgblv.html

[R16] until 等待条件
来源：http://hz.xziqi.cn/gthpqegvwr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jinqigfzy.top/gtmzmqdvel.html

[R17] 数组定义与取值
来源：http://hz.shzxlz.cn/gtozwuvtvy.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.xinyue.icu/gtsgwpaltd.html

[R18] 遍历数组
来源：http://hz.ydjk.org.cn/gtauiyrfrd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.ybcxt.top/gtdqimqjew.html

[R19] 数组长度
来源：http://hz.redwolf501.top/gtovlzlcpx.html

echo "${#arr[@]}"
来源：http://hz.iojbl.cn/gtlzrqiskz.html

[R20] 关联数组（字典）
来源：http://hz.sysykeji.top/gtzmhzoebr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.ydjk.org.cn/gthlvummrw.html

[R21] 字符串长度
来源：http://hz.xuetiantiany.cn/gtzscutfzb.html

echo "${#s}"
来源：http://hz.zhoulong.xyz/gtyoyudnkr.html

[R22] 截取子串
来源：http://hz.zhixingplan.top/gtzgnhulyp.html

echo "${s:0:5}"
来源：http://hz.andypj.xyz/gttbgjeref.html

[R23] 字符串替换
来源：http://hz.aizwys.cn/gtqqpiuhxg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.ywan-chungtsiang.top/gtxomupcjr.html

[R24] 大小写转换
来源：http://hz.jqgfzy.top/gtzahotpie.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yj20258888.top/gtjmvmzynx.html

[R25] 去后缀 / 去前缀
来源：http://hz.aizwys.cn/gtoffckxmi.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.jqgufenzy.top/gthpqxytup.html

[R26] 命令替换
来源：http://hz.cdnleiting.top/gtmtcivxaz.html

now=$(date +%F); echo "$now"
来源：http://hz.cheryme.top/gtglhowssi.html

[R27] 算术展开
来源：http://hz.hfpthk.cn/gtckcqcrpc.html

echo $((1 + 2 * 3))
来源：http://hz.daria6918.cn/gtqdahzxdm.html

[R28] 浮点运算
来源：http://hz.jyoumei.cn/gtvnylfxfb.html

echo "scale=2; 10/3" | bc
来源：http://hz.smart0.xyz/gtstcwvcvb.html

[R29] 定义函数
来源：http://hz.xuanzx.com/gtciwjfzqx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.0kj1m.cn/gtcgwqjeyf.html

[R30] 函数返回状态码
来源：http://hz.zhijiandao.cn/gtiiostwsx.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jqgfzy.top/gtinagmoze.html

[R31] 局部变量
来源：http://hz.hywenlv.cn/gtrjikdlxk.html

f() { local x=1; echo "$x"; }
来源：http://hz.yongpay.top/gtfqqdthdq.html

[R32] 参数个数校验
来源：http://hz.316326.xyz/gtxlbyqulx.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.shzxlz.cn/gtmjcsgcxv.html

[R33] 捕获错误并提示行号
来源：http://hz.zdqjudy.top/gtminmqbqm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zhengqikj.top/gtuxhpwvuc.html

[R34] 退出时清理
来源：http://hz.nanxinkj.top/gtplofhxdu.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.kuanghao11.cn/gtlollxbkf.html

[R35] 后台执行并等待
来源：http://hz.zhoulong.xyz/gtcfjfwnkg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.gzhubu.top/gtygavcacy.html

[R36] 并发执行多个任务
来源：http://hz.hnxiangtu.top/gtmvhqhwad.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jinghuilouyu.cn/gttpsblrbm.html

[R37] 把输出赋给变量
来源：http://hz.ywan-chungtsiang.top/gtuvyrskql.html

files=$(ls -1)
来源：http://hz.wangshuangyany.cn/gtsuafntse.html

[R38] 管道串联
来源：http://hz.hnqzz.top/gtgkhbtwbj.html

cat a.txt | grep -i error | wc -l
来源：http://hz.ivvv.top/gtmazyfnfh.html

[R39] 重定向标准输出与错误
来源：http://hz.cdnleiting.top/gtyfjvvlgv.html

cmd > out.log 2>&1
来源：http://hz.zdqjudy.top/gthqlysjho.html

[R40] 追加写日志
来源：http://hz.ydzc1.top/gtuodogmam.html

echo "log" >> out.log
来源：http://hz.dianchejie.cn/gtaanturyk.html

[R41] 丢弃输出
来源：http://hz.guannengcc.top/gtovmpugld.html

cmd >/dev/null 2>&1
来源：http://hz.fengsongda.top/gtinnjvhcc.html

[R42] 输入重定向
来源：http://hz.jinyuanbaomall.cn/gtavgtjgff.html

wc -l < a.txt
来源：http://hz.52xcode.cn/gtylkuqtjx.html

[R43] 按名字查找文件
来源：http://hz.xingfuxueyuan.xyz/gtrcatfdzf.html

find . -name "*.log" -type f
来源：http://hz.snrcjt.cn/gttwixkvkn.html

[R44] 按修改时间查找
来源：http://hz.hysaishi.cn/gtbytcmfdu.html

find . -mtime -7 -type f
来源：http://hz.ehwqpu.com/gtpvyipdgg.html

[R45] 批量删除
来源：http://hz.cdnleiting.top/gtpdsrpaba.html

find . -name "*.tmp" -delete
来源：http://hz.daria6918.cn/gtkqndtnlt.html

[R46] 递归替换文件内容
来源：http://hz.zhixingplan.top/gtwbrdvjpe.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.dashuyun.cn/gteuouykqz.html

[R47] sed 单行替换
来源：http://hz.ywan-chungtsiang.top/gtvzrfgvwu.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.haohaochexian.top/gtlajqnwww.html

[R48] awk 取指定列
来源：http://hz.jinqigufen.top/gtdvzfcapc.html

awk '{print $1, $3}' a.txt
来源：http://hz.yvedp.cn/gtlczmfbud.html

[R49] awk 带条件
来源：http://hz.pengpengdd.cyou/gtihbreinz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.aizwys.cn/gtejzcdffy.html

[R50] awk 求和
来源：http://hz.gogol.net.cn/gttgoyftmv.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.hysaishi.cn/gtefbfhmhd.html

[R51] 排序去重取前几
来源：http://hz.yanxiufei.cn/gttohkurpx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.sufxvd.cn/gtxsneqjls.html

[R52] 统计行数
来源：http://hz.shanyushiyangtech.top/gtswsjftws.html

wc -l a.txt
来源：http://hz.ivvv.top/gtxfevmizb.html

[R53] 查看文件头与实时尾
来源：http://hz.bjfxy.top/gthxhmiuaq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.hywenlv.cn/gtvorcrtzm.html

[R54] 比较两个文件
来源：http://hz.zhengqikj.top/gtsdcojnpm.html

diff a.txt b.txt
来源：http://hz.sweek.top/gtvkjldxfy.html

[R55] 压缩与解压
来源：http://hz.nanxuanxn.top/gtmvkxaide.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.xingfuxueyuan.xyz/gtchjwilhk.html

[R56] 远程拷贝
来源：http://hz.ybcxt.top/gtdeotnqxq.html

scp file user@host:/path/
来源：http://hz.316326.xyz/gtrdubmyfn.html

[R57] 远程执行命令
来源：http://hz.316326.xyz/gttqvpjoik.html

ssh user@host 'uptime'
来源：http://hz.aizwys.cn/gtivmdyyyj.html

[R58] 下载文件
来源：http://hz.feifeiyinyue.top/gtjknvkdoj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.fengsongda.top/gtusdvvkli.html

[R59] 发 POST JSON
来源：http://hz.shzxlz.cn/gtfinlbayq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.haohaochexian.top/gtzrsuqjud.html

[R60] 只看 HTTP 状态码
来源：http://hz.aizwys.cn/gtyfuahvdd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.sxryk.cn/gtzrzlmyco.html

[R61] 磁盘占用
来源：http://hz.daxiang520.top/gtuiifnfkp.html

df -h;  du -sh *
来源：http://hz.snrcjt.cn/gtoecjhiwq.html

[R62] 找最占空间的文件
来源：http://hz.nwbrower.top/gtkjbstqcz.html

du -ah . | sort -rh | head -10
来源：http://hz.yj202588.top/gtcyrjvscd.html

[R63] 内存与进程
来源：http://hz.jiagoushi.top/gtqesvzqio.html

free -h;  ps aux | grep nginx
来源：http://hz.haohaochexian.top/gtnempdifg.html

[R64] 结束进程
来源：http://hz.meibo888.top/gthacafbps.html

kill -9 $(pgrep -f app.py)
来源：http://hz.zhengqikj.top/gtgdvwfsly.html

[R65] 查看端口占用
来源：http://hz.aibaodan.cn/gtjethbwgk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.kuanghao11.cn/gtwuazdeup.html

[R66] 定时任务
来源：http://hz.jinqigufen.top/gtcdxakwjx.html

crontab -e;  crontab -l
来源：http://hz.cdnleiting.top/gtosazqmtc.html

[R67] 生成随机十六进制串
来源：http://hz.wangdashe.top/gtykalqaoj.html

openssl rand -hex 16
来源：http://hz.xuetiantiany.cn/gtizcofsuf.html

[R68] 计算文件校验值
来源：http://hz.xinyue.icu/gtkbreqzxs.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.jinghuilouyu.cn/gtxkmvtqfx.html

[R69] 生成随机密码
来源：http://hz.yanxiufei.cn/gtwksbcqfz.html

head -c 16 /dev/urandom | base64
来源：http://hz.nwbrower.top/gtktlicajp.html

[R70] 时间戳与互转
来源：http://hz.yj202588.top/gtrmvldgyv.html

date +%s;  date -d @1700000000
来源：http://hz.nanxuanxn.top/gtwfbdpqoh.html

[R71] 日期格式化
来源：http://hz.jinyuanbaomall.cn/gtlcgdfvbk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.shangyingyoupin.top/gtkxjkpojl.html

[R72] 等待端口就绪
来源：http://hz.mhx1999.top/gtjeryxedt.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.yanxiufei.cn/gttkwixbst.html

[R73] 分割大日志
来源：http://hz.fzhhl.top/gtnihdwulc.html

split -l 1000 big.log part_
来源：http://hz.daxiang520.top/gtktvnsrjb.html

[R74] 批量重命名
来源：http://hz.shangyingyoupin.top/gtscfvaidu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.xingfuxueyuan.xyz/gtigpxxlow.html

[R75] 导出环境变量
来源：http://hz.wangdashe.top/gttmblozdx.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.dashuyun.cn/gtzffgouaf.html

[R76] 使用临时文件
来源：http://hz.nanxinkj.top/gtpluktkgj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.nanxuanxn.top/gtotwvuupe.html

[R77] 读取用户输入
来源：http://hz.xingfuxueyuan.xyz/gtvjcrsfaa.html

read -rp "请输入: " ans
来源：http://hz.shuidangran.top/gtwzbtqqnh.html

[R78] 交互式菜单
来源：http://hz.xuetiantiany.cn/gtbwddanho.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.jianghu66.top/gtulkhkvhk.html

[R79] 解析命令行选项
来源：http://hz.hammf.cn/gtitstehtt.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.ydzc1.top/gtrsfkzixr.html

[R80] 查看脚本执行耗时
来源：http://hz.yj202588.top/gttifookqs.html

time ./run.sh
来源：http://hz.yuanzhike.top/gtgxjkbmdf.html

================================================================================
来源：http://hz.bjfxy.top/gthgcbbjly.html

S. C / C++ 专题
来源：http://hz.pycfn.com/gtozkfixdq.html

================================================================================
来源：http://hz.ppjwa.cn/gtxbfqngui.html

[S01] C：Hello World
来源：http://hz.chenjidiqi.icu/gtfdqdzoyq.html

#include <stdio.h>
来源：http://hz.zhaomingkeji.xyz/gtbnsbjvss.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.zhijiandao.cn/gtfxypfmwz.html

[S02] C：变量与格式化输出
来源：http://hz.nwbrower.top/gtbwwagcdh.html

int a = 10; printf("%d\n", a);
来源：http://hz.mhx1999.top/gttrynyvyl.html

[S03] C：读入整数
来源：http://hz.wangshuangyany.cn/gtxwcaxlyv.html

int x; scanf("%d", &x);
来源：http://hz.guowangkeji.top/gtrixbfshq.html

[S04] C：字符串复制
来源：http://hz.nanxinkj.top/gtrchglyos.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.xuanzx.com/gthscurruz.html

[S05] C：字符串长度
来源：http://hz.yvedp.cn/gtuqgxievy.html

strlen(s)
来源：http://hz.dianchejie.cn/gtxqtylrkw.html

[S06] C：字符串比较
来源：http://hz.wangdashe.top/gttdemitkn.html

strcmp(a, b) == 0
来源：http://hz.guowangkeji.top/gtgltbyqzd.html

[S07] C：数组遍历求和
来源：http://hz.zhaomingkeji.xyz/gtoukwgdhe.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.haohaochexian.top/gtsndyqukw.html

[S08] C：动态内存分配与释放
来源：http://hz.ppjwa.cn/gtaixcmzeh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yangfankeji.com/gtvmupsiou.html

[S09] C：结构体定义与初始化
来源：http://hz.yj20258888.top/gtnqxsmflx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.9152youxi.cn/gtkrjnjiru.html

[S10] C：指针与解引用
来源：http://hz.52xcode.cn/gthavootcq.html

int *p = &a;  *p = 5;
来源：http://hz.zycfv.cn/gtvylyxyxi.html

[S11] C：逐行读文件
来源：http://hz.yj202588.top/gtikekfqbs.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.cqqwz.cn/gtyogpnzkd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.tian-w.cn/gtzlvwibli.html

fclose(f);
来源：http://hz.zdqjudy.top/gtblwnoxgo.html

[S12] C：写文件
来源：http://hz.wangshuangyany.cn/gtxdejgahv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.sufxvd.cn/gtckmcsmej.html

[S13] C：宏定义
来源：http://hz.52xcode.cn/gtwehdlqqw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.guannengcc.top/gtypdcjuxl.html

[S14] C：枚举
来源：http://hz.hywenlv.cn/gtwjsmcoum.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.bjfxy.top/gtqlgbxuzf.html

[S15] C：类型转换
来源：http://hz.tian-w.cn/gtwewflkuj.html

(double) a / b
来源：http://hz.yuanzhike.top/gtctbmpjup.html

[S16] C：位操作置位
来源：http://hz.sysykeji.top/gtyjuhtlfx.html

x |= (1 << 3);
来源：http://hz.ywan-chungtsiang.top/gtfzxkyuav.html

[S17] C：安全拼接字符串
来源：http://hz.jiagoushi.top/gtdrlrjoot.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.daxiang520.top/gtuqvyxesm.html

[S18] C：命令行参数
来源：http://hz.zycfv.cn/gtntahqrco.html

int main(int argc, char **argv)
来源：http://hz.jqgfzy.top/gtbgqzvtjw.html

[S19] C：快速排序
来源：http://hz.nanxuanxn.top/gteguicznk.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.xziqi.cn/gtsleykbag.html

[S20] C：二分查找
来源：http://hz.hysaishi.cn/gtneujzbqh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.bjfxy.top/gtrreyzxce.html

[S21] C：字符类别判断
来源：http://hz.havefunace.top/gtjkjherix.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.shanyushiyangkeji.top/gthmnpynyr.html

[S22] C：字符串转数字
来源：http://hz.nanxinkj.top/gtneqjpxxi.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zhongyouzk.top/gtbtmxzfqh.html

[S23] C：随机数
来源：http://hz.shanyushiyangtech.top/gtokstxrpv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.hfpthk.cn/gtkxoflfws.html

[S24] C：获取本地时间
来源：http://hz.tian-w.cn/gtjvglasla.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.dianchejie.cn/gtqiludhrk.html

[S25] C：内存拷贝
来源：http://hz.jlsjyb.cn/gtjxmrlfey.html

memcpy(dst, src, n);
来源：http://hz.mhx1999.top/gthwarmung.html

[S26] C：内存清零
来源：http://hz.ywan-chungtsiang.top/gtqcdahhgh.html

memset(a, 0, sizeof a);
来源：http://hz.daria6918.cn/gtzmvvxgrw.html

[S27] C：定义常量
来源：http://hz.ywan-chungtsiang.top/gtzurmojpg.html

const double PI = 3.14159;
来源：http://hz.dianchejie.cn/gtzdteslhr.html

[S28] C：静态变量
来源：http://hz.aizwys.cn/gtfptkjbll.html

static int counter = 0;
来源：http://hz.mhx1999.top/gthenpfoxb.html

[S29] C：变参函数
来源：http://hz.hnqzz.top/gtdixpmttw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.xuetiantiany.cn/gthtghyiua.html

[S30] C：头文件保护
来源：http://hz.zhijiandao.cn/gtfmzuonzg.html

#ifndef X_H
来源：http://hz.tian-w.cn/gtpycfxbbx.html

#define X_H
来源：http://hz.yvedp.cn/gtfjtkwszm.html

#endif
来源：http://hz.jiagoushi.top/gtskepwuua.html

[S31] C++：Hello World
来源：http://hz.xuanzx.com/gtfsowhrhu.html

#include <iostream>
来源：http://hz.ywan-chungtsiang.top/gtkazpewfk.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.jyoumei.cn/gtyrbxlher.html

[S32] C++：字符串
来源：http://hz.shzxlz.cn/gtiokgokws.html

std::string s = "hi";  s += "!";
来源：http://hz.pycfn.com/gtayktnldt.html

[S33] C++：vector 增删
来源：http://hz.9152youxi.cn/gtjpknizcp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.xuanzx.com/gtzacterkh.html

[S34] C++：遍历 vector
来源：http://hz.nanxuanxn.top/gtfvobrelh.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yangfankeji.com/gtwnyageaf.html

[S35] C++：map
来源：http://hz.sysykeji.top/gtprrsuzxa.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.fengsongda.top/gtbxpslzlq.html

[S36] C++：unordered_map
来源：http://hz.yangfankeji.com/gtivpfgmle.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.nanxuanxn.top/gtrgmndqjz.html

[S37] C++：set
来源：http://hz.gzhubu.top/gtxzfrfirw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.cqqwz.cn/gtvijnchgt.html

[S38] C++：排序
来源：http://hz.smart0.xyz/gtipefzxpc.html

std::sort(v.begin(), v.end());
来源：http://hz.ywan-chungtsiang.top/gtjdlnstgv.html

[S39] C++：自定义比较器排序
来源：http://hz.zhiwuduotai.top/gtmehmjmsu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.havefunace.top/gtbporrhwk.html

[S40] C++：查找元素
来源：http://hz.kuanghao11.cn/gtbuekmsxi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.fengsongda.top/gtdnipmdhe.html

[S41] C++：类与构造函数
来源：http://hz.xuetiantiany.cn/gtmvszefzt.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.tian-w.cn/gtscmgnlky.html

[S42] C++：继承与虚函数
来源：http://hz.wangdashe.top/gtswqhsrri.html

class B : public Base { public: void f() override {} };
来源：http://hz.cdnleiting.top/gtlisjcjxs.html

[S43] C++：智能指针
来源：http://hz.wangdashe.top/gtehnkgsoe.html

auto p = std::make_unique<int>(5);
来源：http://hz.chenjidiqi.icu/gtakojlqzd.html

[S44] C++：引用传参
来源：http://hz.sxryk.cn/gtlwjsiwfx.html

void inc(int &x) { ++x; }
来源：http://hz.yangfankeji.com/gtszzgqkkh.html

[S45] C++：lambda
来源：http://hz.c1oappe.top/gtfkfpneap.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.nanxinkj.top/gtmgorhftx.html

[S46] C++：函数模板
来源：http://hz.jinqigfzy.top/gtbyfkykgs.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.aizwys.cn/gtywwtthzp.html

[S47] C++：结构化绑定遍历
来源：http://hz.pycfn.com/gtavuefnzz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.ywan-chungtsiang.top/gtiqlhbrea.html

[S48] C++：逐行读文件
来源：http://hz.pengpengdd.cyou/gtpvwpftbv.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.ywan-chungtsiang.top/gtxfgkbuyv.html

while (std::getline(in, line)) { }
来源：http://hz.jinqigfzy.top/gtiecgpknb.html

[S49] C++：写文件
来源：http://hz.hnqzz.top/gtouixhtnt.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.jlsjyb.cn/gtfwhcolol.html

[S50] C++：格式化数字
来源：http://hz.guannengcc.top/gtmrwndzvf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.wangdashe.top/gtfokmjxug.html

[S51] C++：显式类型转换
来源：http://hz.yangfankeji.com/gtsizxtgib.html

static_cast<double>(a) / b
来源：http://hz.ywan-chungtsiang.top/gtudukchfl.html

[S52] C++：const 与 noexcept
来源：http://hz.jqgufenzy.top/gtimugrffa.html

int size() const noexcept { return n_; }
来源：http://hz.zhaomingkeji.xyz/gtphrhdnhz.html

[S53] C++：移动语义
来源：http://hz.shanyushiyangkeji.top/gtauwkaadn.html

std::vector<int> w = std::move(v);
来源：http://hz.zdqjudy.top/gttjnkasjt.html

[S54] C++：异常处理
来源：http://hz.vqdsnc.cn/gttjjouecz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.wangshuangyany.cn/gtmnmvwyte.html

[S55] C++：结构化绑定
来源：http://hz.xingfuxueyuan.xyz/gtlntvbkzd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.52xcode.cn/gttuzfqktw.html

[S56] C++：optional
来源：http://hz.bjfxy.top/gtuntajxof.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.andypj.xyz/gtlqqlavuz.html

[S57] C++：编译期常量
来源：http://hz.wangdashe.top/gtxdztcfwj.html

constexpr int N = 10;
来源：http://hz.gogol.net.cn/gtliaxqunj.html

[S58] C++：命名空间
来源：http://hz.sufxvd.cn/gtzuweyqys.html

namespace ns { int f() { return 1; } }
来源：http://hz.andypj.xyz/gtsjbnwtwe.html

[S59] C++：静态断言
来源：http://hz.jinqigufen.top/gtphqzszbr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.zycfv.cn/gtmeqcupkw.html

[S60] C++：遍历并删除元素
来源：http://hz.shanyushiyangtech.top/gtwziqoula.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.ydzc1.top/gtwmcecdcn.html

================================================================================
来源：http://hz.c1oappe.top/gtqmkzouee.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.gogol.net.cn/gtmflfgsyw.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtfqwkeqxr.html

[T01] Kotlin：Hello World
来源：http://hz.aizwys.cn/gtenvtnbjq.html

println("Hello")
来源：http://hz.gotoacloud.top/gtgucgbylk.html

[T02] Kotlin：变量
来源：http://hz.ppjwa.cn/gthgozvvpd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.cucudq.cn/gtwpdahuoo.html

[T03] Kotlin：字符串模板
来源：http://hz.c1oappe.top/gtcyxkmlir.html

"值: $b"
来源：http://hz.hammf.cn/gtzjffedvt.html

[T04] Kotlin：空安全
来源：http://hz.yuanzhike.top/gtkobqmldy.html

val n: String? = null;  n?.length
来源：http://hz.jianghu66.top/gtvbefxsbx.html

[T05] Kotlin：when 表达式
来源：http://hz.daxiang520.top/gtqjezuxrh.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yangfankeji.com/gtnpgosjoq.html

[T06] Kotlin：集合映射
来源：http://hz.c1oappe.top/gttyqahhpq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jinghuilouyu.cn/gtgcjdysjd.html

[T07] Kotlin：集合过滤
来源：http://hz.xinyue.icu/gtpgldqvdz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.cheryme.top/gtazyjduvl.html

[T08] Kotlin：数据类
来源：http://hz.nwbrower.top/gtxglisgej.html

data class User(val name: String, val age: Int)
来源：http://hz.andypj.xyz/gtznnsliov.html

[T09] Kotlin：扩展函数
来源：http://hz.shanyushiyangkeji.top/gtohbzwnue.html

fun String.exclaim() = this + "!"
来源：http://hz.xziqi.cn/gtwfsslzgu.html

[T10] Kotlin：默认参数
来源：http://hz.bjfxy.top/gtvuperghh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jyoumei.cn/gtjlxowkkx.html

[T11] Kotlin：协程
来源：http://hz.xingfuxueyuan.xyz/gtkgxctnhj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.shzxlz.cn/gtdysgfjrv.html

[T12] Kotlin：解构声明
来源：http://hz.ywan-chungtsiang.top/gtdpvgxraq.html

val (a, b) = Pair(1, 2)
来源：http://hz.fengsongda.top/gtrkduvfqv.html

[T13] Kotlin：只读 Map
来源：http://hz.shangyingyoupin.top/gtaybebyum.html

val m = mapOf("a" to 1)
来源：http://hz.zhijiandao.cn/gtuxpggolq.html

[T14] Kotlin：循环
来源：http://hz.haohaochexian.top/gtmpawwckx.html

for (i in 1..10) println(i)
来源：http://hz.ybcxt.top/gtipfwnvuy.html

[T15] Kotlin：接口
来源：http://hz.shanyushiyangkeji.top/gtrxczfumz.html

interface Shape { fun area(): Double }
来源：http://hz.ydjk.org.cn/gtirktsupo.html

[T16] Swift：Hello World
来源：http://hz.shzxlz.cn/gtallqeyyw.html

print("Hello")
来源：http://hz.wangshuangyany.cn/gtswhsiuoa.html


<!-- 参考信息 -->