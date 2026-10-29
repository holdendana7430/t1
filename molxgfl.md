代发 wailian999

name="${1:-default}"
来源：http://read.share.zdbjq.cn/Article/details/ghbfmotpx.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/gcnvycqzy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gzoldzdql.sHtML

[R07] if 判断文件
来源：http://3g.fehbvm.com/Article/details/gajpaalle.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.hesvh.cn/Article/details/gejqptjxr.sHtML

[R08] 数值比较
来源：http://mobile.fehbvm.com/Article/details/gyxzvydud.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gcdcdjenv.sHtML

[R09] 字符串比较
来源：http://3g.hesvh.cn/Article/details/gkcjjxjao.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.hesvh.cn/Article/details/gsevrjclz.sHtML

[R10] 正则匹配
来源：http://baike.hesvh.cn/Article/details/grcoeeqzj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fehbvm.com/Article/details/gmlitcujo.sHtML

[R11] case 多分支
来源：http://www.blog.hesvh.cn/Article/details/gilmcrfxb.sHtML

case "$1" in
来源：http://www.m.share.hesvh.cn/Article/details/gxiwprcnj.sHtML

start) echo "启动" ;;
来源：http://www.blog.fehbvm.com/Article/details/gdxjstvfb.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fehbvm.com/Article/details/gprtqwblm.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fehbvm.com/Article/details/goqyjlfgj.sHtML

esac
来源：http://baike.fehbvm.com/Article/details/gwzhopptf.sHtML

[R12] for 遍历文件
来源：http://mobile.fehbvm.com/Article/details/grrzmefag.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fehbvm.com/Article/details/gmfjrofpf.sHtML

[R13] for 计数循环
来源：http://wap.zdbjq.cn/Article/details/ggsggbnjv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gfjooeqtq.sHtML

[R14] C 风格 for
来源：http://baike.fehbvm.com/Article/details/gxmdhwptq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gqkucocud.sHtML

[R15] while 逐行读文件
来源：http://3g.hesvh.cn/Article/details/gmsahoear.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fehbvm.com/Article/details/gcbcindrd.sHtML

[R16] until 等待条件
来源：http://www.blog.fehbvm.com/Article/details/gbfbqyqib.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/girilpmtl.sHtML

[R17] 数组定义与取值
来源：http://baike.hesvh.cn/Article/details/gfmvykmiz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fehbvm.com/Article/details/gqqsnzbwc.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/gkgrigxuc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.hesvh.cn/Article/details/goszdugzj.sHtML

[R19] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/grlwgwszd.sHtML

echo "${#arr[@]}"
来源：http://wap.zdbjq.cn/Article/details/gkcqiadgl.sHtML

[R20] 关联数组（字典）
来源：http://wap.fehbvm.com/Article/details/gemodbkfn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.zdbjq.cn/Article/details/gocbvbvlr.sHtML

[R21] 字符串长度
来源：http://read.share.zdbjq.cn/Article/details/ghkjzmwlg.sHtML

echo "${#s}"
来源：http://wap.fehbvm.com/Article/details/guyuxfvsc.sHtML

[R22] 截取子串
来源：http://blog.hesvh.cn/Article/details/geaychukt.sHtML

echo "${s:0:5}"
来源：http://mobile.zdbjq.cn/Article/details/glkvndyem.sHtML

[R23] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/guoywmxju.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fehbvm.com/Article/details/gdjcbmsgp.sHtML

[R24] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gzgxrrodp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.zdbjq.cn/Article/details/gfvbrakof.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fehbvm.com/Article/details/gbyolfgps.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fehbvm.com/Article/details/gtnzmymub.sHtML

[R26] 命令替换
来源：http://www.blog.fehbvm.com/Article/details/gwpljtqlh.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.zdbjq.cn/Article/details/gqrshlfnk.sHtML

[R27] 算术展开
来源：http://read.share.hesvh.cn/Article/details/goyhvrchw.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.zdbjq.cn/Article/details/gcrfgevrl.sHtML

[R28] 浮点运算
来源：http://www.m.share.zdbjq.cn/Article/details/gqhktnbln.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.zdbjq.cn/Article/details/gifqoqpmi.sHtML

[R29] 定义函数
来源：http://wap.zdbjq.cn/Article/details/glapptxsl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fehbvm.com/Article/details/gvegenbfl.sHtML

[R30] 函数返回状态码
来源：http://www.blog.hesvh.cn/Article/details/gporpfrsb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fehbvm.com/Article/details/gzjimkaon.sHtML

[R31] 局部变量
来源：http://baike.fehbvm.com/Article/details/gejewsdim.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.hesvh.cn/Article/details/gxwkhbght.sHtML

[R32] 参数个数校验
来源：http://www.blog.hesvh.cn/Article/details/gdqjlkzsm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gzhazczux.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.zdbjq.cn/Article/details/gcedbktqr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.zdbjq.cn/Article/details/gqmhptfwu.sHtML

[R34] 退出时清理
来源：http://blog.hesvh.cn/Article/details/gxwqszsfb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gufxnhhng.sHtML

[R35] 后台执行并等待
来源：http://www.share.hesvh.cn/Article/details/gswyopbsz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fehbvm.com/Article/details/ghtmkczpf.sHtML

[R36] 并发执行多个任务
来源：http://mobile.zdbjq.cn/Article/details/ginmekqxe.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.zdbjq.cn/Article/details/ghchkntiz.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fehbvm.com/Article/details/gxzuluwme.sHtML

files=$(ls -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gaeyqaeiz.sHtML

[R38] 管道串联
来源：http://blog.zdbjq.cn/Article/details/ghymvdryf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.hesvh.cn/Article/details/gcitltfnl.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.zdbjq.cn/Article/details/gsqxzlhcp.sHtML

cmd > out.log 2>&1
来源：http://baike.fehbvm.com/Article/details/gpuzwudxd.sHtML

[R40] 追加写日志
来源：http://wap.hesvh.cn/Article/details/gjilrppdv.sHtML

echo "log" >> out.log
来源：http://m.share.fehbvm.com/Article/details/gqeeuprca.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fehbvm.com/Article/details/gscobluqd.sHtML

cmd >/dev/null 2>&1
来源：http://wap.hesvh.cn/Article/details/guoqakblz.sHtML

[R42] 输入重定向
来源：http://mobile.zdbjq.cn/Article/details/gavuxskdz.sHtML

wc -l < a.txt
来源：http://m.share.fehbvm.com/Article/details/gvmmzgtpc.sHtML

[R43] 按名字查找文件
来源：http://read.share.zdbjq.cn/Article/details/gwysmkavl.sHtML

find . -name "*.log" -type f
来源：http://baike.zdbjq.cn/Article/details/gxrlwuwmw.sHtML

[R44] 按修改时间查找
来源：http://blog.fehbvm.com/Article/details/grjpwpfoz.sHtML

find . -mtime -7 -type f
来源：http://wap.hesvh.cn/Article/details/gjyvvyyde.sHtML

[R45] 批量删除
来源：http://blog.hesvh.cn/Article/details/gnlkxxxob.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fehbvm.com/Article/details/gcxzbxkxu.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/gqnlmifsz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fehbvm.com/Article/details/gnkkkgnsy.sHtML

[R47] sed 单行替换
来源：http://baike.hesvh.cn/Article/details/gkzufcbcb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gdvuqkolu.sHtML

[R48] awk 取指定列
来源：http://m.share.fehbvm.com/Article/details/gjrpkzlol.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gwkbqrybd.sHtML

[R49] awk 带条件
来源：http://www.m.share.hesvh.cn/Article/details/gmclvafrw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fehbvm.com/Article/details/geqfypdqu.sHtML

[R50] awk 求和
来源：http://m.share.fehbvm.com/Article/details/gvtifnsfi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gakgtzmur.sHtML

[R51] 排序去重取前几
来源：http://read.share.hesvh.cn/Article/details/gxcvlcnhc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.hesvh.cn/Article/details/ggynukiod.sHtML

[R52] 统计行数
来源：http://blog.hesvh.cn/Article/details/gghreqopo.sHtML

wc -l a.txt
来源：http://m.share.zdbjq.cn/Article/details/gfosbhwtz.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.hesvh.cn/Article/details/ghdvviyyk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.hesvh.cn/Article/details/gdzvkiwhx.sHtML

[R54] 比较两个文件
来源：http://wap.zdbjq.cn/Article/details/galdbrtxy.sHtML

diff a.txt b.txt
来源：http://www.m.share.hesvh.cn/Article/details/gwyhxwqzh.sHtML

[R55] 压缩与解压
来源：http://baike.hesvh.cn/Article/details/gwifsleux.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fehbvm.com/Article/details/ggadmilfu.sHtML

[R56] 远程拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gvyvgyozg.sHtML

scp file user@host:/path/
来源：http://3g.hesvh.cn/Article/details/gihnvsljq.sHtML

[R57] 远程执行命令
来源：http://read.share.hesvh.cn/Article/details/gzdxnpyck.sHtML

ssh user@host 'uptime'
来源：http://blog.hesvh.cn/Article/details/gixaxtqek.sHtML

[R58] 下载文件
来源：http://3g.hesvh.cn/Article/details/goqakoojw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fehbvm.com/Article/details/gafmxxawq.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/gvkjgmfou.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.zdbjq.cn/Article/details/gsxgucqly.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gnvczqwzd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.hesvh.cn/Article/details/gfgqqcivv.sHtML

[R61] 磁盘占用
来源：http://blog.zdbjq.cn/Article/details/glvcpdphw.sHtML

df -h;  du -sh *
来源：http://3g.zdbjq.cn/Article/details/gvnqrljmk.sHtML

[R62] 找最占空间的文件
来源：http://baike.hesvh.cn/Article/details/gzmzytbgy.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fehbvm.com/Article/details/giebefzmy.sHtML

[R63] 内存与进程
来源：http://read.share.zdbjq.cn/Article/details/gryyugfgi.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fehbvm.com/Article/details/gzinbsgfa.sHtML

[R64] 结束进程
来源：http://www.m.share.zdbjq.cn/Article/details/gdvdmwdbp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fehbvm.com/Article/details/gyjzhmahe.sHtML

[R65] 查看端口占用
来源：http://blog.fehbvm.com/Article/details/gtlnefuwa.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.zdbjq.cn/Article/details/gdnjdcfey.sHtML

[R66] 定时任务
来源：http://m.share.hesvh.cn/Article/details/gcvojlbfa.sHtML

crontab -e;  crontab -l
来源：http://www.share.hesvh.cn/Article/details/gmjwiggta.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fehbvm.com/Article/details/gbwnidqln.sHtML

openssl rand -hex 16
来源：http://3g.hesvh.cn/Article/details/guqbofxpa.sHtML

[R68] 计算文件校验值
来源：http://www.blog.zdbjq.cn/Article/details/gmoucpkbd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/gxedgtxol.sHtML

[R69] 生成随机密码
来源：http://www.share.zdbjq.cn/Article/details/glxjtobis.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.zdbjq.cn/Article/details/gizifwxba.sHtML

[R70] 时间戳与互转
来源：http://blog.fehbvm.com/Article/details/ggocvatzs.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/gtsotvvkr.sHtML

[R71] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gjmdsoazv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fehbvm.com/Article/details/gqibazvce.sHtML

[R72] 等待端口就绪
来源：http://blog.fehbvm.com/Article/details/gobfmmmeo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gxfrqqijc.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/gzvzmitsp.sHtML

split -l 1000 big.log part_
来源：http://3g.fehbvm.com/Article/details/guwbafcbr.sHtML

[R74] 批量重命名
来源：http://3g.fehbvm.com/Article/details/gvhfldvej.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gwefjekox.sHtML

[R75] 导出环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gpihlnckq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fehbvm.com/Article/details/gskcnljvo.sHtML

[R76] 使用临时文件
来源：http://mobile.fehbvm.com/Article/details/geskxdwcr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gxewyceay.sHtML

[R77] 读取用户输入
来源：http://blog.hesvh.cn/Article/details/gmowdjwry.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/gnzprktpn.sHtML

[R78] 交互式菜单
来源：http://www.m.share.zdbjq.cn/Article/details/geibsnykb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fehbvm.com/Article/details/gbzjmyuah.sHtML

[R79] 解析命令行选项
来源：http://wap.fehbvm.com/Article/details/ghthdvgej.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.hesvh.cn/Article/details/gnfhgewci.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fehbvm.com/Article/details/gbypebfca.sHtML

time ./run.sh
来源：http://baike.zdbjq.cn/Article/details/gvkvdojgl.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghgqetdfl.sHtML

S. C / C++ 专题
来源：http://www.share.zdbjq.cn/Article/details/gvntvryeh.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwbjkripl.sHtML

[S01] C：Hello World
来源：http://www.share.fehbvm.com/Article/details/gbfpbvktd.sHtML

#include <stdio.h>
来源：http://blog.zdbjq.cn/Article/details/gvydcyqzz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.hesvh.cn/Article/details/gmkbdakxg.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.zdbjq.cn/Article/details/gxxbuwmqa.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fehbvm.com/Article/details/gzuaakyod.sHtML

[S03] C：读入整数
来源：http://wap.zdbjq.cn/Article/details/gssgrlksm.sHtML

int x; scanf("%d", &x);
来源：http://3g.hesvh.cn/Article/details/gtsfywtxr.sHtML

[S04] C：字符串复制
来源：http://baike.fehbvm.com/Article/details/glhwpscro.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.hesvh.cn/Article/details/gbylaihov.sHtML

[S05] C：字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/geieisslg.sHtML

strlen(s)
来源：http://blog.fehbvm.com/Article/details/gjjhlassi.sHtML

[S06] C：字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gqbdexmqf.sHtML

strcmp(a, b) == 0
来源：http://baike.zdbjq.cn/Article/details/gbzpfouan.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/gbpsdvarf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.zdbjq.cn/Article/details/gnfmxaxdy.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fehbvm.com/Article/details/gauajygwo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/gxhzjoppr.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.hesvh.cn/Article/details/ggqffznch.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fehbvm.com/Article/details/gqooyiwpn.sHtML

[S10] C：指针与解引用
来源：http://blog.hesvh.cn/Article/details/gbmlldevh.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.zdbjq.cn/Article/details/gkgbytipj.sHtML

[S11] C：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gqttacmnp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.zdbjq.cn/Article/details/gsptppucb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fehbvm.com/Article/details/gcbrpneoe.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/gcjvelciq.sHtML

[S12] C：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gcxosqxxs.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gzwjwqxol.sHtML

[S13] C：宏定义
来源：http://mobile.zdbjq.cn/Article/details/gaayqnfis.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.hesvh.cn/Article/details/gmoxavpfn.sHtML

[S14] C：枚举
来源：http://mobile.fehbvm.com/Article/details/gomsfkrhk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.zdbjq.cn/Article/details/gpkybhdyv.sHtML

[S15] C：类型转换
来源：http://baike.fehbvm.com/Article/details/gsmevxulh.sHtML

(double) a / b
来源：http://read.share.zdbjq.cn/Article/details/gwpxobflb.sHtML

[S16] C：位操作置位
来源：http://3g.zdbjq.cn/Article/details/gdrnwxxft.sHtML

x |= (1 << 3);
来源：http://www.blog.fehbvm.com/Article/details/gazimjasa.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gwjvmbsdq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.hesvh.cn/Article/details/gwzsranmv.sHtML

[S18] C：命令行参数
来源：http://www.share.hesvh.cn/Article/details/gqkvxnqaw.sHtML

int main(int argc, char **argv)
来源：http://www.blog.zdbjq.cn/Article/details/gzcqmuuvx.sHtML

[S19] C：快速排序
来源：http://m.share.fehbvm.com/Article/details/gsvkqkapc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gbpvrqqca.sHtML

[S20] C：二分查找
来源：http://www.m.share.hesvh.cn/Article/details/gjlcxutya.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gccakmvzv.sHtML

[S21] C：字符类别判断
来源：http://www.share.hesvh.cn/Article/details/gsdsdyvdh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.hesvh.cn/Article/details/giouhkchf.sHtML

[S22] C：字符串转数字
来源：http://www.share.hesvh.cn/Article/details/gofnwwixd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.hesvh.cn/Article/details/gsyektchr.sHtML

[S23] C：随机数
来源：http://m.share.fehbvm.com/Article/details/gmuwzmmyp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.zdbjq.cn/Article/details/gdkfurmgk.sHtML

[S24] C：获取本地时间
来源：http://read.share.hesvh.cn/Article/details/ghdvibebn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.hesvh.cn/Article/details/ghhkrfuup.sHtML

[S25] C：内存拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gnvakgwsu.sHtML

memcpy(dst, src, n);
来源：http://wap.hesvh.cn/Article/details/gcgwnixkh.sHtML

[S26] C：内存清零
来源：http://www.share.zdbjq.cn/Article/details/gyzptvsbt.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fehbvm.com/Article/details/gvlqkzhoo.sHtML

[S27] C：定义常量
来源：http://blog.fehbvm.com/Article/details/glnzosnwt.sHtML

const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gkfpqpvhn.sHtML

[S28] C：静态变量
来源：http://read.share.zdbjq.cn/Article/details/ggjuwsywy.sHtML

static int counter = 0;
来源：http://baike.hesvh.cn/Article/details/gdmittwof.sHtML

[S29] C：变参函数
来源：http://www.blog.zdbjq.cn/Article/details/gwkkqgykf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/gqyhknrrf.sHtML

[S30] C：头文件保护
来源：http://www.m.share.hesvh.cn/Article/details/gqbhefrrs.sHtML

#ifndef X_H
来源：http://mobile.hesvh.cn/Article/details/gzxlxvylb.sHtML

#define X_H
来源：http://baike.fehbvm.com/Article/details/glxqtkbmv.sHtML

#endif
来源：http://mobile.zdbjq.cn/Article/details/gmvxmyqga.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gnlqkpeew.sHtML

#include <iostream>
来源：http://www.share.fehbvm.com/Article/details/gwwptiwoh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/gqddxxqut.sHtML

[S32] C++：字符串
来源：http://3g.zdbjq.cn/Article/details/gqzhxtkkr.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.zdbjq.cn/Article/details/gcfpckfkq.sHtML

[S33] C++：vector 增删
来源：http://blog.fehbvm.com/Article/details/gtyrvpupz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/giaupvewt.sHtML

[S34] C++：遍历 vector
来源：http://www.share.hesvh.cn/Article/details/gvynehgvz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.zdbjq.cn/Article/details/gegdyvjex.sHtML

[S35] C++：map
来源：http://mobile.zdbjq.cn/Article/details/gwellhrkq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gdtalsgvi.sHtML

[S36] C++：unordered_map
来源：http://mobile.zdbjq.cn/Article/details/gzinjilio.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gcuzbzccr.sHtML

[S37] C++：set
来源：http://m.share.zdbjq.cn/Article/details/gbonvcaty.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.hesvh.cn/Article/details/gdxikrkfz.sHtML

[S38] C++：排序
来源：http://mobile.fehbvm.com/Article/details/gcbpxwtxz.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gldiwfrix.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fehbvm.com/Article/details/gosqqejmt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.zdbjq.cn/Article/details/gmpzwypzi.sHtML

[S40] C++：查找元素
来源：http://blog.hesvh.cn/Article/details/gblmsoczp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fehbvm.com/Article/details/gvecdzcdw.sHtML

[S41] C++：类与构造函数
来源：http://baike.hesvh.cn/Article/details/gppxtbarf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fehbvm.com/Article/details/gpactqmic.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fehbvm.com/Article/details/gvqesyfls.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fehbvm.com/Article/details/gaaspouwz.sHtML

[S43] C++：智能指针
来源：http://baike.fehbvm.com/Article/details/grnriavzd.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/gbkrwyhld.sHtML

[S44] C++：引用传参
来源：http://www.share.hesvh.cn/Article/details/gqojlbcqb.sHtML

void inc(int &x) { ++x; }
来源：http://baike.zdbjq.cn/Article/details/gqdnqbadx.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/grbyqyjzz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.zdbjq.cn/Article/details/gabzocgam.sHtML

[S46] C++：函数模板
来源：http://baike.hesvh.cn/Article/details/gxysloarg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.hesvh.cn/Article/details/gvcqxvgmp.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.hesvh.cn/Article/details/ghmwmppdt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.hesvh.cn/Article/details/glwbqzmah.sHtML

[S48] C++：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gvvrtdjuk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.zdbjq.cn/Article/details/ghykcxlhj.sHtML

while (std::getline(in, line)) { }
来源：http://blog.zdbjq.cn/Article/details/gcmcnrrha.sHtML

[S49] C++：写文件
来源：http://www.share.hesvh.cn/Article/details/ggreazbpz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.hesvh.cn/Article/details/girszpdnx.sHtML

[S50] C++：格式化数字
来源：http://read.share.fehbvm.com/Article/details/gqpwsibpk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gkywrfkbn.sHtML

[S51] C++：显式类型转换
来源：http://read.share.hesvh.cn/Article/details/gzkbbglxr.sHtML

static_cast<double>(a) / b
来源：http://3g.hesvh.cn/Article/details/gydrxdiwh.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fehbvm.com/Article/details/gewcbdvfy.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.zdbjq.cn/Article/details/gygobmbpk.sHtML

[S53] C++：移动语义
来源：http://wap.fehbvm.com/Article/details/gxyduwble.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fehbvm.com/Article/details/gruhcpgso.sHtML

[S54] C++：异常处理
来源：http://baike.hesvh.cn/Article/details/gvmjqjuha.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fehbvm.com/Article/details/gsesnyntf.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fehbvm.com/Article/details/gtztfkmiu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gxnyhjvbj.sHtML

[S56] C++：optional
来源：http://blog.hesvh.cn/Article/details/gwgcaupms.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.zdbjq.cn/Article/details/glqtyfdnm.sHtML

[S57] C++：编译期常量
来源：http://wap.fehbvm.com/Article/details/gwmhiuyum.sHtML

constexpr int N = 10;
来源：http://3g.zdbjq.cn/Article/details/grcfneudj.sHtML

[S58] C++：命名空间
来源：http://mobile.hesvh.cn/Article/details/gmxuxzxaq.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.zdbjq.cn/Article/details/glkstupjy.sHtML

[S59] C++：静态断言
来源：http://wap.zdbjq.cn/Article/details/gujbyazuk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.zdbjq.cn/Article/details/ginjtimbb.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.hesvh.cn/Article/details/gzgwouzed.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.hesvh.cn/Article/details/gkxqdebjn.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gftdccizy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gxevaixfu.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gyvcnxjrc.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fehbvm.com/Article/details/gtkojdxyu.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gnewyugvi.sHtML

[T02] Kotlin：变量
来源：http://wap.fehbvm.com/Article/details/gdgjptbzp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.zdbjq.cn/Article/details/gdbdiwgza.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.hesvh.cn/Article/details/gyyhstigu.sHtML

"值: $b"
来源：http://3g.fehbvm.com/Article/details/gtovdsztj.sHtML

[T04] Kotlin：空安全
来源：http://wap.hesvh.cn/Article/details/grcrecser.sHtML

val n: String? = null;  n?.length
来源：http://m.share.hesvh.cn/Article/details/gauajpoyr.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.hesvh.cn/Article/details/gnjbtmmmu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.zdbjq.cn/Article/details/gcoqxfykz.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.zdbjq.cn/Article/details/gggxoswyu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/ghxgykswa.sHtML


<!-- 参考信息 -->