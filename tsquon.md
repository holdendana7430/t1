代发 wailian999

echo "${#arr[@]}"
来源：http://hz.chenlongwang.top/gtfddflkdm.html

[R20] 关联数组（字典）
来源：http://hz.vqdsnc.cn/gtdkbusocb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.0kj1m.cn/gtoyiwbxvf.html

[R21] 字符串长度
来源：http://hz.xziqi.cn/gtdzyhcapk.html

echo "${#s}"
来源：http://hz.ydzc1.top/gttjxxibxn.html

[R22] 截取子串
来源：http://hz.tianlin.xyz/gtqxhqzyjz.html

echo "${s:0:5}"
来源：http://hz.quarkkingdee.top/gtmiyqpbiz.html

[R23] 字符串替换
来源：http://hz.jinyuanbaomall.cn/gtqnhvraon.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.mhx1999.top/gtoubuwwiv.html

[R24] 大小写转换
来源：http://hz.cashguo.top/gtsaycphej.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.jlsjyb.cn/gtzhnbcrzg.html

[R25] 去后缀 / 去前缀
来源：http://hz.tian-w.cn/gttxuoeaqg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.cashguo.top/gtghqbfwzq.html

[R26] 命令替换
来源：http://hz.wangshuangyany.cn/gtzbimyfnq.html

now=$(date +%F); echo "$now"
来源：http://hz.yueranfly.top/gtqqfxgbty.html

[R27] 算术展开
来源：http://hz.yonumen.top/gtppxjlzmi.html

echo $((1 + 2 * 3))
来源：http://hz.zycfv.cn/gtsttptwkj.html

[R28] 浮点运算
来源：http://hz.zhixingplan.top/gtjqpdyjjj.html

echo "scale=2; 10/3" | bc
来源：http://hz.jinghuilouyu.cn/gtxjgnbdet.html

[R29] 定义函数
来源：http://hz.quarkkingdee.top/gtgsahcuuh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.cashguo.top/gtvtksfwwy.html

[R30] 函数返回状态码
来源：http://hz.mhx1999.top/gtmnpujdde.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.zdqjudy.top/gtmmaswzwl.html

[R31] 局部变量
来源：http://hz.ybcxt.top/gtgvwshycu.html

f() { local x=1; echo "$x"; }
来源：http://hz.yanxiufei.cn/gtdwezsnyh.html

[R32] 参数个数校验
来源：http://hz.hammf.cn/gtvqqezuud.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.nanxuanxn.top/gtlbywuxup.html

[R33] 捕获错误并提示行号
来源：http://hz.yueranfly.top/gtuchlgkrt.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.tianlin.xyz/gtormgnqft.html

[R34] 退出时清理
来源：http://hz.yuxming.cn/gtqfbkzdqn.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yj20258.top/gtsdaikouu.html

[R35] 后台执行并等待
来源：http://hz.52xcode.cn/gtqybbonof.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.gogol.net.cn/gtchnmcntv.html

[R36] 并发执行多个任务
来源：http://hz.jinyuanbaomall.cn/gtqkombunr.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.tian-w.cn/gtqrbgvpwe.html

[R37] 把输出赋给变量
来源：http://hz.bjfxy.top/gtpeibyzlh.html

files=$(ls -1)
来源：http://hz.tanke756.top/gtneozbptq.html

[R38] 管道串联
来源：http://hz.jqgufenzy.top/gtoutjircg.html

cat a.txt | grep -i error | wc -l
来源：http://hz.sysykeji.top/gttxcwwelt.html

[R39] 重定向标准输出与错误
来源：http://hz.yj202588.top/gtqgfpjmwp.html

cmd > out.log 2>&1
来源：http://hz.tian-w.cn/gtfspgnfhu.html

[R40] 追加写日志
来源：http://hz.xingfuxueyuan.xyz/gttlnmwbgz.html

echo "log" >> out.log
来源：http://hz.bjfxy.top/gtoukkgdhx.html

[R41] 丢弃输出
来源：http://hz.xziqi.cn/gtcmyklski.html

cmd >/dev/null 2>&1
来源：http://hz.yanxiufei.cn/gtjenpznlc.html

[R42] 输入重定向
来源：http://hz.shanyushiyangtech.top/gtrvrashsz.html

wc -l < a.txt
来源：http://hz.nwbrower.top/gtnzhfwuoj.html

[R43] 按名字查找文件
来源：http://hz.andypj.xyz/gtzegenxwp.html

find . -name "*.log" -type f
来源：http://hz.hywenlv.cn/gtigfukzgz.html

[R44] 按修改时间查找
来源：http://hz.ehwqpu.com/gtuqydnnse.html

find . -mtime -7 -type f
来源：http://hz.haohaochexian.top/gtellzxgqj.html

[R45] 批量删除
来源：http://hz.daxiang520.top/gtnbjkmqbs.html

find . -name "*.tmp" -delete
来源：http://hz.zhixingplan.top/gtivuldjoy.html

[R46] 递归替换文件内容
来源：http://hz.xinyue.icu/gtwpexxbiq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yj20258888.top/gtkpgweuyn.html

[R47] sed 单行替换
来源：http://hz.jyoumei.cn/gtorwcwxtj.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.gogol.net.cn/gtxisjdrgr.html

[R48] awk 取指定列
来源：http://hz.dianchejie.cn/gtkkadlash.html

awk '{print $1, $3}' a.txt
来源：http://hz.nwbrower.top/gtgtlsrkvo.html

[R49] awk 带条件
来源：http://hz.fzhhl.top/gtktwluxzy.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.xingfuxueyuan.xyz/gtwbcowdci.html

[R50] awk 求和
来源：http://hz.daria6918.cn/gtlavzlwui.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.hywenlv.cn/gtfggmzqcd.html

[R51] 排序去重取前几
来源：http://hz.meibo888.top/gtpnpzbbbi.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jqgfzy.top/gtdoabbcug.html

[R52] 统计行数
来源：http://hz.yj20258.top/gtqqsidklb.html

wc -l a.txt
来源：http://hz.cucudq.cn/gtiohatmqa.html

[R53] 查看文件头与实时尾
来源：http://hz.ppjwa.cn/gtxihxpvai.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.nanxinkj.top/gtaevoczjr.html

[R54] 比较两个文件
来源：http://hz.9152youxi.cn/gtybyflqkc.html

diff a.txt b.txt
来源：http://hz.jiagoushi.top/gtpwngdwzm.html

[R55] 压缩与解压
来源：http://hz.chenlongwang.top/gtkqwfsevr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.aibaodan.cn/gtppjzkrtb.html

[R56] 远程拷贝
来源：http://hz.fengsongda.top/gtmnazccke.html

scp file user@host:/path/
来源：http://hz.cqqwz.cn/gtwtaiqznk.html

[R57] 远程执行命令
来源：http://hz.smart0.xyz/gtbegrbuor.html

ssh user@host 'uptime'
来源：http://hz.chenjidiqi.icu/gtguyjmzfb.html

[R58] 下载文件
来源：http://hz.yueranfly.top/gtdbqulhpi.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.nanxuanxn.top/gtkfemnsiy.html

[R59] 发 POST JSON
来源：http://hz.yueranfly.top/gtqcconbxj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.hywenlv.cn/gttnnybmqp.html

[R60] 只看 HTTP 状态码
来源：http://hz.c1oappe.top/gtggherycg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.hfpthk.cn/gtizsnnpbx.html

[R61] 磁盘占用
来源：http://hz.gogol.net.cn/gtcrlcsybz.html

df -h;  du -sh *
来源：http://hz.nanxinkj.top/gtfjpjxcuw.html

[R62] 找最占空间的文件
来源：http://hz.ydzc1.top/gtxuifdbow.html

du -ah . | sort -rh | head -10
来源：http://hz.zycfv.cn/gtysnytfco.html

[R63] 内存与进程
来源：http://hz.yuxming.cn/gtcgdjgnxi.html

free -h;  ps aux | grep nginx
来源：http://hz.yj20258.top/gtxzygtros.html

[R64] 结束进程
来源：http://hz.yongpay.top/gtexdaybic.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yangfankeji.com/gtoeleogrc.html

[R65] 查看端口占用
来源：http://hz.gotoacloud.top/gtpsgxmfai.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.zhengqikj.top/gtipokskah.html

[R66] 定时任务
来源：http://hz.nanxinkj.top/gtzxqxdiuq.html

crontab -e;  crontab -l
来源：http://hz.zdqjudy.top/gtfeoekpeu.html

[R67] 生成随机十六进制串
来源：http://hz.yvedp.cn/gtrkqhbvhz.html

openssl rand -hex 16
来源：http://hz.xuanzx.com/gtegcglvqm.html

[R68] 计算文件校验值
来源：http://hz.9152youxi.cn/gtzyqevimj.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.pengpengdd.cyou/gtqfiuygez.html

[R69] 生成随机密码
来源：http://hz.hywenlv.cn/gtmktmynuq.html

head -c 16 /dev/urandom | base64
来源：http://hz.52xcode.cn/gtgwssczrc.html

[R70] 时间戳与互转
来源：http://hz.jqgfzy.top/gtzxunbiln.html

date +%s;  date -d @1700000000
来源：http://hz.nwbrower.top/gtkxrlntew.html

[R71] 日期格式化
来源：http://hz.316326.xyz/gtudqvcvfw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.ivvv.top/gtpbhgxjzk.html

[R72] 等待端口就绪
来源：http://hz.yj20258.top/gtzlfwkzgu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jianghu66.top/gtexbcaamb.html

[R73] 分割大日志
来源：http://hz.cucudq.cn/gtevtaqwqw.html

split -l 1000 big.log part_
来源：http://hz.feifeiyinyue.top/gtcxpbzdxs.html

[R74] 批量重命名
来源：http://hz.jqgfzy.top/gtikrrebdw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.cucudq.cn/gtpvlfhljv.html

[R75] 导出环境变量
来源：http://hz.jlsjyb.cn/gtmthqppmx.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.316326.xyz/gthyktnhwd.html

[R76] 使用临时文件
来源：http://hz.daria6918.cn/gtcoojijqi.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.316326.xyz/gtwquabocs.html

[R77] 读取用户输入
来源：http://hz.yuxming.cn/gtrfswzkbw.html

read -rp "请输入: " ans
来源：http://hz.yangfankeji.com/gtviheulwe.html

[R78] 交互式菜单
来源：http://hz.ybcxt.top/gtlzbxfriv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.feifeiyinyue.top/gtcdnmdqmw.html

[R79] 解析命令行选项
来源：http://hz.iojbl.cn/gtsxhplezf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.tanke756.top/gtkpuaqdgx.html

[R80] 查看脚本执行耗时
来源：http://hz.aibaodan.cn/gtswwiqvhs.html

time ./run.sh
来源：http://hz.smart0.xyz/gtsimaxjyj.html

================================================================================
来源：http://hz.zhoulong.xyz/gtkjflumty.html

S. C / C++ 专题
来源：http://hz.aizwys.cn/gtpoitthda.html

================================================================================
来源：http://hz.52xcode.cn/gtszdwzeec.html

[S01] C：Hello World
来源：http://hz.sweek.top/gtqezypnnl.html

#include <stdio.h>
来源：http://hz.shanyushiyangkeji.top/gtkstjadxq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.vqdsnc.cn/gtgkzahxms.html

[S02] C：变量与格式化输出
来源：http://hz.jianghu66.top/gtyrxfkjho.html

int a = 10; printf("%d\n", a);
来源：http://hz.jinqigufen.top/gtycpjdccp.html

[S03] C：读入整数
来源：http://hz.kuanghao11.cn/gtsawznkxj.html

int x; scanf("%d", &x);
来源：http://hz.birdmap.top/gtzfsbvmwh.html

[S04] C：字符串复制
来源：http://hz.ydzc1.top/gtmdhidpda.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.svipenyu.cn/gtcshdwdli.html

[S05] C：字符串长度
来源：http://hz.xuanzx.com/gtoxelskoy.html

strlen(s)
来源：http://hz.feifeiyinyue.top/gtsebuxnwm.html

[S06] C：字符串比较
来源：http://hz.svipenyu.cn/gtyrfourlh.html

strcmp(a, b) == 0
来源：http://hz.shanyushiyangkeji.top/gtlvoptlva.html

[S07] C：数组遍历求和
来源：http://hz.redwolf501.top/gttpesaqeq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.ydzc1.top/gtyzhhspxf.html

[S08] C：动态内存分配与释放
来源：http://hz.hfpthk.cn/gtqpwzhcof.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.zhengqikj.top/gtbrsbmsgo.html

[S09] C：结构体定义与初始化
来源：http://hz.zhongyouzk.top/gtvuvhasky.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.tanke756.top/gtkfaygitg.html

[S10] C：指针与解引用
来源：http://hz.jiagoushi.top/gtkuwfbrnt.html

int *p = &a;  *p = 5;
来源：http://hz.kuanghao11.cn/gtqecotpsw.html

[S11] C：逐行读文件
来源：http://hz.xuanzx.com/gtsjeyeigp.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.c1oappe.top/gtsjoffcei.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.kuanghao11.cn/gtxilecibq.html

fclose(f);
来源：http://hz.havefunace.top/gtuwnwshqo.html

[S12] C：写文件
来源：http://hz.fengsongda.top/gtzgxufnjj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.xziqi.cn/gtynpyxuam.html

[S13] C：宏定义
来源：http://hz.dianchejie.cn/gtxacwmjso.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.tian-w.cn/gtalixewxv.html

[S14] C：枚举
来源：http://hz.wangdashe.top/gthwevonoc.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yj20258888.top/gtovnnndyi.html

[S15] C：类型转换
来源：http://hz.havefunace.top/gtzjkrhpag.html

(double) a / b
来源：http://hz.daxiang520.top/gttqnqxwye.html

[S16] C：位操作置位
来源：http://hz.shanyushiyangkeji.top/gtbphlshhg.html

x |= (1 << 3);
来源：http://hz.zhoulong.xyz/gtygboqaov.html

[S17] C：安全拼接字符串
来源：http://hz.quarkkingdee.top/gtshotjvch.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.yuanzhike.top/gtakizslwe.html

[S18] C：命令行参数
来源：http://hz.hnxiangtu.top/gtsdhpkmha.html

int main(int argc, char **argv)
来源：http://hz.gzhubu.top/gtykppagth.html

[S19] C：快速排序
来源：http://hz.gogol.net.cn/gtnjnkheqp.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.chenjidiqi.icu/gtymeymjto.html

[S20] C：二分查找
来源：http://hz.jlsjyb.cn/gtozanvezs.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.chenzaomai.com/gtnzsyjljc.html

[S21] C：字符类别判断
来源：http://hz.daxiang520.top/gtkqjyfmwt.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.sysykeji.top/gtjwnpzpta.html

[S22] C：字符串转数字
来源：http://hz.vqdsnc.cn/gtcdzixmkw.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.shanyushiyangkeji.top/gtaoegdvqw.html

[S23] C：随机数
来源：http://hz.0kj1m.cn/gtnkmkoiig.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.svipenyu.cn/gtjtumkaxi.html

[S24] C：获取本地时间
来源：http://hz.xuetiantiany.cn/gtfjhoatix.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.jiagoushi.top/gtdwqtdhnz.html

[S25] C：内存拷贝
来源：http://hz.chenjidiqi.icu/gtmimsjwdr.html

memcpy(dst, src, n);
来源：http://hz.hnqzz.top/gtdjacgzpr.html

[S26] C：内存清零
来源：http://hz.9152youxi.cn/gtbfwpfofl.html

memset(a, 0, sizeof a);
来源：http://hz.gogol.net.cn/gtseqbxeve.html

[S27] C：定义常量
来源：http://hz.c1oappe.top/gtbwgiqvzw.html

const double PI = 3.14159;
来源：http://hz.shzxlz.cn/gtywekozbg.html

[S28] C：静态变量
来源：http://hz.hnxiangtu.top/gtebhcawsm.html

static int counter = 0;
来源：http://hz.daria6918.cn/gtnjfhzwub.html

[S29] C：变参函数
来源：http://hz.ybcxt.top/gtnahsbuqg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.meibo888.top/gtpobksnaw.html

[S30] C：头文件保护
来源：http://hz.jinqigfzy.top/gtphwtcjel.html

#ifndef X_H
来源：http://hz.havefunace.top/gtrivxxzlx.html

#define X_H
来源：http://hz.meibo888.top/gtvxaudwqe.html

#endif
来源：http://hz.shzxlz.cn/gtfjxeovrp.html

[S31] C++：Hello World
来源：http://hz.yueranfly.top/gtpffafrfh.html

#include <iostream>
来源：http://hz.hnqzz.top/gtwylbzgtn.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yanxiufei.cn/gtdxsfkjkt.html

[S32] C++：字符串
来源：http://hz.shangyingyoupin.top/gtmqgfbcxr.html

std::string s = "hi";  s += "!";
来源：http://hz.aibaodan.cn/gtspaluugg.html

[S33] C++：vector 增删
来源：http://hz.mhx1999.top/gtryaudwvk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.ydzc1.top/gtbxvokbza.html

[S34] C++：遍历 vector
来源：http://hz.yuxming.cn/gtkweqbxdi.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.dianchejie.cn/gtwtswweij.html

[S35] C++：map
来源：http://hz.daria6918.cn/gtlvgeeluv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jqgufenzy.top/gthgmjtlhl.html

[S36] C++：unordered_map
来源：http://hz.hnqzz.top/gtqgxnnrmi.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jiagoushi.top/gtiozoanzq.html

[S37] C++：set
来源：http://hz.chenlongwang.top/gtitdxyvkg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.cdnleiting.top/gttiwlrpgu.html

[S38] C++：排序
来源：http://hz.guannengcc.top/gtqsphtjdh.html

std::sort(v.begin(), v.end());
来源：http://hz.zhongyouzk.top/gtmqetmtqd.html

[S39] C++：自定义比较器排序
来源：http://hz.xinyue.icu/gthguxxqzp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.9152youxi.cn/gtrlxpvggc.html

[S40] C++：查找元素
来源：http://hz.jqgufenzy.top/gtsedvqgiq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.0kj1m.cn/gtkuoruqlv.html

[S41] C++：类与构造函数
来源：http://hz.yvedp.cn/gtkdnktwjc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.zhengqikj.top/gtupbgoqyy.html

[S42] C++：继承与虚函数
来源：http://hz.zhixingplan.top/gtqaiarssu.html

class B : public Base { public: void f() override {} };
来源：http://hz.9152youxi.cn/gtbpkkbyrr.html

[S43] C++：智能指针
来源：http://hz.hysaishi.cn/gtucvdmpas.html

auto p = std::make_unique<int>(5);
来源：http://hz.guannengcc.top/gtcshtrxuo.html

[S44] C++：引用传参
来源：http://hz.zhixingplan.top/gtmjhisgos.html

void inc(int &x) { ++x; }
来源：http://hz.tianlin.xyz/gtoogecwmv.html

[S45] C++：lambda
来源：http://hz.cqqwz.cn/gttdwceswr.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.hysaishi.cn/gtzekjzlhv.html

[S46] C++：函数模板
来源：http://hz.ehwqpu.com/gtgzxyexzn.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.ywan-chungtsiang.top/gtkhuxovqa.html

[S47] C++：结构化绑定遍历
来源：http://hz.sweek.top/gtoupywwor.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.aizwys.cn/gtbyelcprc.html

[S48] C++：逐行读文件
来源：http://hz.yuxming.cn/gtzjdkxpmw.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.daxiang520.top/gtgluterds.html

while (std::getline(in, line)) { }
来源：http://hz.shuidangran.top/gtnnvqjtuq.html

[S49] C++：写文件
来源：http://hz.52xcode.cn/gtleldgfpi.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.aizwys.cn/gtnjgtjbip.html

[S50] C++：格式化数字
来源：http://hz.gzhubu.top/gtdgaupvrm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jinqigufen.top/gtmtaekkkx.html

[S51] C++：显式类型转换
来源：http://hz.hongshengwenyu.top/gtsabikaay.html

static_cast<double>(a) / b
来源：http://hz.jinghuilouyu.cn/gtfbxqbrcp.html

[S52] C++：const 与 noexcept
来源：http://hz.andypj.xyz/gtxlikkrxw.html

int size() const noexcept { return n_; }
来源：http://hz.zhijiandao.cn/gtfepirrxc.html

[S53] C++：移动语义
来源：http://hz.sufxvd.cn/gtirmvnfei.html

std::vector<int> w = std::move(v);
来源：http://hz.xziqi.cn/gtizsoifnk.html

[S54] C++：异常处理
来源：http://hz.ydzc1.top/gtoffsowox.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.zhoulong.xyz/gtvxtyqfvn.html

[S55] C++：结构化绑定
来源：http://hz.hywenlv.cn/gtmqldgdqz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.ppjwa.cn/gttlcumfxg.html

[S56] C++：optional
来源：http://hz.ywan-chungtsiang.top/gttjtxsydk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.xinyue.icu/gtmpapdhrm.html

[S57] C++：编译期常量
来源：http://hz.cdnleiting.top/gttrstwosq.html

constexpr int N = 10;
来源：http://hz.xuanzx.com/gttkbvtpge.html

[S58] C++：命名空间
来源：http://hz.shangyingyoupin.top/gtzxiyqyze.html

namespace ns { int f() { return 1; } }
来源：http://hz.zycfv.cn/gtreldemkj.html

[S59] C++：静态断言
来源：http://hz.feifeiyinyue.top/gtwffwopwg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.hongshengwenyu.top/gttjuchpkn.html

[S60] C++：遍历并删除元素
来源：http://hz.sweek.top/gthvgeafsa.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.redwolf501.top/gtfukhdzet.html

================================================================================
来源：http://hz.gogol.net.cn/gtercujvym.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zycfv.cn/gtpzhxdccm.html

================================================================================
来源：http://hz.316326.xyz/gtrjotqyuu.html

[T01] Kotlin：Hello World
来源：http://hz.guowangkeji.top/gtyjvqrrdu.html

println("Hello")
来源：http://hz.hongshengwenyu.top/gtxadaykzy.html

[T02] Kotlin：变量
来源：http://hz.aibaodan.cn/gtyertnduo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.redwolf501.top/gtusrriohw.html

[T03] Kotlin：字符串模板
来源：http://hz.hysaishi.cn/gttkcrqzwj.html

"值: $b"
来源：http://hz.sweek.top/gtgchitxxo.html

[T04] Kotlin：空安全
来源：http://hz.yongpay.top/gtqbxpkeye.html

val n: String? = null;  n?.length
来源：http://hz.xuanzx.com/gthysnqanr.html

[T05] Kotlin：when 表达式
来源：http://hz.shanyushiyangkeji.top/gtquiwxqig.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.chenzaomai.com/gtrngwgzuk.html

[T06] Kotlin：集合映射
来源：http://hz.zycfv.cn/gtmymcocfx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.quarkkingdee.top/gtshotvjhk.html

[T07] Kotlin：集合过滤
来源：http://hz.aibaodan.cn/gtoegvqdgs.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.fzhhl.top/gtyeppfwjq.html

[T08] Kotlin：数据类
来源：http://hz.gogol.net.cn/gtnnzmnovp.html

data class User(val name: String, val age: Int)
来源：http://hz.iojbl.cn/gthhsvejac.html

[T09] Kotlin：扩展函数
来源：http://hz.pycfn.com/gtcdeypcab.html

fun String.exclaim() = this + "!"
来源：http://hz.sysykeji.top/gtpltcnrjh.html

[T10] Kotlin：默认参数
来源：http://hz.yvedp.cn/gtphjlbbkd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.havefunace.top/gtkndywcov.html

[T11] Kotlin：协程
来源：http://hz.guannengcc.top/gtqnbohqgq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.cashguo.top/gtirupapis.html

[T12] Kotlin：解构声明
来源：http://hz.sxryk.cn/gthkxfkbdd.html

val (a, b) = Pair(1, 2)
来源：http://hz.vqdsnc.cn/gtxumcehzb.html

[T13] Kotlin：只读 Map
来源：http://hz.wangdashe.top/gtvrbndjjb.html

val m = mapOf("a" to 1)
来源：http://hz.yj202588.top/gtopskntet.html

[T14] Kotlin：循环
来源：http://hz.yvedp.cn/gtlqzzrmix.html

for (i in 1..10) println(i)
来源：http://hz.fzhhl.top/gtlqbqpgda.html

[T15] Kotlin：接口
来源：http://hz.cucudq.cn/gtfukwebum.html

interface Shape { fun area(): Double }
来源：http://hz.zhiwuduotai.top/gtgiprfrmv.html

[T16] Swift：Hello World
来源：http://hz.gaohongyu789.top/gtkvbvaujr.html

print("Hello")
来源：http://hz.316326.xyz/gtihnmqize.html

[T17] Swift：变量与常量
来源：http://hz.xuetiantiany.cn/gtigddiwmp.html

var a = 1;  let b = 2
来源：http://hz.yuanzhike.top/gtuldaobsm.html

[T18] Swift：字符串插值
来源：http://hz.zhijiandao.cn/gtlgqxkahf.html

"值: \(b)"
来源：http://hz.316326.xyz/gtrhfbgnby.html

[T19] Swift：可选绑定
来源：http://hz.kuanghao11.cn/gtjysllcji.html

if let n = opt { print(n) }
来源：http://hz.pycfn.com/gtycwuirql.html

[T20] Swift：数组操作
来源：http://hz.yueranfly.top/gtaafdzlxi.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.sweek.top/gtirunbyzc.html

[T21] Swift：遍历
来源：http://hz.wangshuangyany.cn/gtjbrhiode.html

for x in a { print(x) }
来源：http://hz.cashguo.top/gtunwbzhap.html

[T22] Swift：字典
来源：http://hz.tian-w.cn/gtwonxivjs.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.haohaochexian.top/gtckzsvgmg.html


<!-- 参考信息 -->