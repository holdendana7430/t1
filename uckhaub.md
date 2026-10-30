代发 wailian999

esac
来源：http://wap.fanxiaobao.xyz/Article/details/gemrbfizz.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkfuhqog.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/grnukpcor.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/glfntewvw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbpdntyl.sHtML

[R14] C 风格 for
来源：http://m.share.fanxiaobao.xyz/Article/details/ghsptmhhg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gsurxzkfz.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/goikmntnh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gqgdpbqzm.sHtML

[R16] until 等待条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gztptagln.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gianmdrmc.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/gpuriupha.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwahtwis.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkwsckdw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geofmhevk.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gekqphapl.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gddulpxnv.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvqbqnzw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gtcyfxvpk.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwkjmibl.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gguaelxre.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhqompxb.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gyoywbsns.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhahnhvk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gqhkhicbn.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/glaxhyuav.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gvadnkthq.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdjqaaan.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gvnimrvrb.sHtML

[R26] 命令替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqmvnxxj.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/gkdeawbyi.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/gqyjujvui.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fanxiaobao.xyz/Article/details/garqdvuto.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gdomqbgkx.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/giwmfrjwp.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gutevhnfb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gsquzqisx.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gnkewbfzv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggefkzunx.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gpxhjhvtp.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsryvjbkn.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/ggnmdfifj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyddrfnwt.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gacbqeeib.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkttpzir.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gewjkmfgp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gztqcpfvp.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvyrvnvfc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/ggdvtrqdj.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/glyiywejc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdujgzba.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gjoxzvclb.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfauyuen.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/gdibqmfta.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlyygkxs.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbqyytke.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzijicuo.sHtML

[R40] 追加写日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjhxcrau.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/gqpcuwrle.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/gvslwsgkw.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gojwctonk.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjkxzipq.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrmdutsp.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/gqcbwtkjx.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/grkqhyutl.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gcefcrbnb.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpatdqkl.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gcmkmcshs.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/gfemvqpmd.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gaiqusdhn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvaqwdhb.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhxndqwq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnndbzpq.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gcapouesj.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gyulfarup.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gobxvnuea.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/gnhlhefhs.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhtypoab.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gppnxxyrx.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/gcnuwknty.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnrktyfa.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/gaeozcutr.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gldvfpybm.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybvsqfrd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/gphgztagu.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gejuxnhgo.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gajksshar.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/gqetnotte.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/gthmqkgve.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/guitrsijt.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/glbbnrdcl.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/gtbytjyje.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtxtqjbh.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyiyozzgm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmksatmrx.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gquxvgohi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/gjylfklnq.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgzeavll.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxvezpjn.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/glcqcolvl.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gjxvboryj.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/gyfupzamw.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggyrznltr.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gqzsjoyod.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gvcvtaypm.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdhhpzmk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/glpkiegkn.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gkcwsogaj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gfsgmdcxv.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/ggjntalyn.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gfziuldts.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gfseygibq.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvefpmmx.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/gntwxisxv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/goikzudxk.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/gwyhndcwh.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gcpbpdzgb.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqusiyiw.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/gnqiidvuc.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzrgilom.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpvbzdyv.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzjldxsx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltaqmfco.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gmfucxghp.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpueyvdkl.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gklqcqbqp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjjgstzv.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxyksbxf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhtjrpuh.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdrduxvu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmvnnlso.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnaylyvc.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/gipadkpjj.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gymhiaokh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbdsrdrp.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxvgouji.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzsxxtwi.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gexsszdry.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnedxydy.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfhsmxdo.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gmwwpwmbw.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gxxanjlwe.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlggixrf.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gczguwzgb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/glxvreseh.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gbpluojbs.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlvhvfbz.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkjsryfo.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnjfhadi.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/gcubgqemp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/gapzhonsr.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtqgnyhs.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhrinjww.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/ghyakrycm.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxwlbpob.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkotdfckg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/gairjobyj.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkmpbwyr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gneacwgbr.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/gsrscozpe.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gpqmeaxas.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/gvozpjdlr.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvroerzj.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gpvwffita.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/gxtxpuzna.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/glyfcxtnp.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gdamuitwx.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajzjskdl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gnxqcioxd.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzyspjhl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gjayerhye.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gpavmytiz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/gmlpylwih.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqdevyrv.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/ghooddejh.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/ghmtdxjnt.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfkiuyuo.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geowabrbb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gueplzxfc.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gmrsfwrhd.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmoxcjbxo.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gplrkmdfa.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gmkdydmeg.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gkaofvtdo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqhwndxz.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gszxdesch.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/gpwwwmfxf.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gdthpvcqe.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdijipgbu.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmpmsnot.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutulhmwx.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gelsrcxuc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekzgxoqf.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrylekso.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/guheebipt.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjkndnpq.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqwkuovk.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gdmqjqoag.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkydgqavm.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/grahkevqm.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytinjksy.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdoyxdjt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnnrtgcv.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/garwgtjwi.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gnaccmphm.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaoujyoch.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/gdwjnftsp.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gwucqqroo.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojmilmjb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfxxbtcf.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gblhdyulp.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/gptazooot.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gulwxwmps.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwggjcvqt.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcdzonwv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjirmgkfz.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gscxaobss.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjanpkti.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghyruwfjq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpiduvixl.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/gilxlwhhe.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/grigaliad.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkhuecfp.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwoszzgl.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gegprlpsy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqwkhmxi.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/gklbvjqzp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gsygkjcta.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcwzupfp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfnqfidh.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gywczkiew.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxglygxg.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gterripnl.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gqjrpflsa.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/gntijrazb.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkszffozs.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdfccvey.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsokqhtoo.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/gaxbbvejf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gosdjpneg.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlrbhlpn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdjaynvc.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gkfntnipl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzofgzcbt.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklkebyxi.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/goqpavcyo.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/goafbnwdd.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gxrsginsf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrzocgwz.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gysdxdims.sHtML

static_cast<double>(a) / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbxlqald.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/gexzcbype.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fanxiaobao.xyz/Article/details/gsfzkbaxq.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwmvzbcj.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fanxiaobao.xyz/Article/details/gkxyvdlzx.sHtML

[S54] C++：异常处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/giozdehnj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqgmtfmt.sHtML

[S55] C++：结构化绑定
来源：http://wap.fanxiaobao.xyz/Article/details/ggwdtrisg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gdcokfoui.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/gespiyuhf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fanxiaobao.xyz/Article/details/ggmshsgwz.sHtML

[S57] C++：编译期常量
来源：http://wap.fanxiaobao.xyz/Article/details/gjthbvvsv.sHtML

constexpr int N = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gewadfxoa.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcmnhfco.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gdsufpfih.sHtML

[S59] C++：静态断言
来源：http://baike.fanxiaobao.xyz/Article/details/gbsobbcqn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/giksoufpr.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvxwbduf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gzeznciht.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxypjyzk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbdjkjwj.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlpkgmxr.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/grpsanxdn.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gxrdbywzd.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwqxwnls.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fanxiaobao.xyz/Article/details/gntmasvoo.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gkoumkrjo.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gcnhqzwdo.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/ghzfbzjtn.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gywkictbm.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gegpxoqiy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fanxiaobao.xyz/Article/details/gqrdymvue.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/guiezqqzc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxafmjpyz.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gunaxcsug.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fanxiaobao.xyz/Article/details/gjezzorwq.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gltxdwrfh.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtpcrfktb.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxlebetr.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtjxbpzd.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fanxiaobao.xyz/Article/details/gtlycxuoq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fanxiaobao.xyz/Article/details/gkzcuemdq.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gboaffsvt.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkvbxnni.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fanxiaobao.xyz/Article/details/gcwgjemgn.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gicdecdjs.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gnqgnltrm.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fanxiaobao.xyz/Article/details/ghxdjecxu.sHtML

[T14] Kotlin：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnhlgxom.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjntjljqm.sHtML


<!-- 参考信息 -->