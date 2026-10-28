代发 wailian999

[Q78] 当前时间
来源：http://hz.smart0.xyz/gtgvmsdnvr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.daria6918.cn/gthffcuhik.html

[Q79] 字符串拼接
来源：http://hz.jinyuanbaomall.cn/gtwiaousns.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.shangyingyoupin.top/gtsqtzdahs.html

[Q80] 字符串截取
来源：http://hz.yj202588.top/gtclwwjwsk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.wangdashe.top/gtjcymrwna.html

[Q81] 字符串替换
来源：http://hz.jqgfzy.top/gtznnottao.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.ywan-chungtsiang.top/gtuybhyjrz.html

[Q82] 字符长度与字节长度
来源：http://hz.jqgfzy.top/gteqvqxmfr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yj20258.top/gtwneslioo.html

[Q83] 大小写转换
来源：http://hz.chenzaomai.com/gtlsytjifr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.nwbrower.top/gtrcqbspme.html

[Q84] 去除首尾空格
来源：http://hz.yanxiufei.cn/gtdfqknegy.html

SELECT TRIM(name) FROM users;
来源：http://hz.redwolf501.top/gtxzdmaalr.html

[Q85] 数值取整
来源：http://hz.mhx1999.top/gtpwxzeyes.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.yueranfly.top/gtgkgshkgg.html

[Q86] 读取 JSON 字段
来源：http://hz.jinqigfzy.top/gtkcjobhcp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.kuanghao11.cn/gtptoowfpm.html

[Q87] JSON 字段做条件
来源：http://hz.yj20258.top/gttlobvkng.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.vqdsnc.cn/gtobnzerrz.html

[Q88] 行转列（条件聚合）
来源：http://hz.xuetiantiany.cn/gtarrrpgcw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.cucudq.cn/gtmezmgjmb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.0kj1m.cn/gteevrkqok.html

[Q89] 判断表是否存在
来源：http://hz.daria6918.cn/gtazxyames.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.cdnleiting.top/gtoxfonhip.html

[Q90] 生成序号列
来源：http://hz.jinqigfzy.top/gtyskoxdij.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.sufxvd.cn/gthscdfomo.html

================================================================================
来源：http://hz.jqgfzy.top/gtwxyisnnr.html

R. Bash 专题
来源：http://hz.daxiang520.top/gtpwnzlfvy.html

================================================================================
来源：http://hz.hfpthk.cn/gthhoejxky.html

[R01] shebang 与严格模式
来源：http://hz.tianlin.xyz/gtbpkhpicr.html

#!/usr/bin/env bash
来源：http://hz.ppjwa.cn/gtgfzwjzag.html

set -euo pipefail
来源：http://hz.feifeiyinyue.top/gtgbrsguwb.html

[R02] 变量赋值与使用
来源：http://hz.jqgufenzy.top/gtdncxhcam.html

name="Tom"; echo "$name"
来源：http://hz.daxiang520.top/gtuxsxkukm.html

[R03] 只读变量
来源：http://hz.yuanzhike.top/gtplgtaahp.html

readonly PI=3.14
来源：http://hz.ivvv.top/gtacddaogb.html

[R04] 位置参数
来源：http://hz.guannengcc.top/gtqsttxcwq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.aibaodan.cn/gtkcihdpyj.html

[R05] 参数默认值
来源：http://hz.gaohongyu789.top/gtxcwasmaq.html

name="${1:-default}"
来源：http://hz.iojbl.cn/gtfzjvtjpi.html

[R06] 判断命令是否存在
来源：http://hz.fzhhl.top/gtsppblfqn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.bjfxy.top/gtqummcopy.html

[R07] if 判断文件
来源：http://hz.zhixingplan.top/gttkoxwgtz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.quarkkingdee.top/gtqevgbsiy.html

[R08] 数值比较
来源：http://hz.yongpay.top/gtmvltuila.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jianghu66.top/gtdeoyuiby.html

[R09] 字符串比较
来源：http://hz.yuanzhike.top/gtipuivlel.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.daria6918.cn/gtwtpmnizu.html

[R10] 正则匹配
来源：http://hz.sysykeji.top/gtughplfot.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.guowangkeji.top/gtmxkngiwk.html

[R11] case 多分支
来源：http://hz.hnxiangtu.top/gtipzoowwl.html

case "$1" in
来源：http://hz.tianlin.xyz/gtnfjaexsu.html

start) echo "启动" ;;
来源：http://hz.nanxinkj.top/gtvnzqojkf.html

stop)  echo "停止" ;;
来源：http://hz.fengsongda.top/gttipehgwf.html

*)     echo "未知命令" ;;
来源：http://hz.jyoumei.cn/gtqsfkzujf.html

esac
来源：http://hz.yj202588.top/gteiuyysjw.html

[R12] for 遍历文件
来源：http://hz.aizwys.cn/gtlcrwjsvj.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yueranfly.top/gtnlfvxgkd.html

[R13] for 计数循环
来源：http://hz.tianlin.xyz/gtwvxrvenx.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.cheryme.top/gtpiavmoup.html

[R14] C 风格 for
来源：http://hz.yuanzhike.top/gtuwdxgvgq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.cheryme.top/gtfzhpwviy.html

[R15] while 逐行读文件
来源：http://hz.shanyushiyangtech.top/gtvfxzgfxb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.chenzaomai.com/gtnivvrihd.html

[R16] until 等待条件
来源：http://hz.andypj.xyz/gtdzegnoez.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.shanyushiyangtech.top/gtylevqxkk.html

[R17] 数组定义与取值
来源：http://hz.cdnleiting.top/gtrvqgsqzj.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yanxiufei.cn/gtfwdyhpkf.html

[R18] 遍历数组
来源：http://hz.hywenlv.cn/gtczrckmos.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.sysykeji.top/gtoiemqyqm.html

[R19] 数组长度
来源：http://hz.0kj1m.cn/gtordvafis.html

echo "${#arr[@]}"
来源：http://hz.jlsjyb.cn/gtlvqrvwvp.html

[R20] 关联数组（字典）
来源：http://hz.shzxlz.cn/gtxxjrxgce.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.hysaishi.cn/gtgwbquuhk.html

[R21] 字符串长度
来源：http://hz.cucudq.cn/gtgbzyfgoc.html

echo "${#s}"
来源：http://hz.chenjidiqi.icu/gtoaggqicr.html

[R22] 截取子串
来源：http://hz.wangdashe.top/gtxiaxsrao.html

echo "${s:0:5}"
来源：http://hz.yanxiufei.cn/gtcuzibapl.html

[R23] 字符串替换
来源：http://hz.ybcxt.top/gtxcikammj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.cheryme.top/gtwpmkgybm.html

[R24] 大小写转换
来源：http://hz.hnxiangtu.top/gtpnhsrjge.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.kuanghao11.cn/gtyjukuuhe.html

[R25] 去后缀 / 去前缀
来源：http://hz.smart0.xyz/gthyujlbtb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.vqdsnc.cn/gtiitpwfiz.html

[R26] 命令替换
来源：http://hz.shuidangran.top/gthfibswep.html

now=$(date +%F); echo "$now"
来源：http://hz.9152youxi.cn/gtlxpjkkvr.html

[R27] 算术展开
来源：http://hz.guowangkeji.top/gtplaqhaja.html

echo $((1 + 2 * 3))
来源：http://hz.yuanzhike.top/gtwtuifojk.html

[R28] 浮点运算
来源：http://hz.meibo888.top/gtmqjjbqpk.html

echo "scale=2; 10/3" | bc
来源：http://hz.guowangkeji.top/gtdfcbveef.html

[R29] 定义函数
来源：http://hz.haohaochexian.top/gtmszlskkv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.gzhubu.top/gtynffqfrx.html

[R30] 函数返回状态码
来源：http://hz.nwbrower.top/gtjubzhtfh.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.shangyingyoupin.top/gtorldeamz.html

[R31] 局部变量
来源：http://hz.aizwys.cn/gtqrfvotmu.html

f() { local x=1; echo "$x"; }
来源：http://hz.nwbrower.top/gtgvcwzjpo.html

[R32] 参数个数校验
来源：http://hz.fzhhl.top/gtnnmglswf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.gogol.net.cn/gtmctralfl.html

[R33] 捕获错误并提示行号
来源：http://hz.xziqi.cn/gtkzzadbvm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zhoulong.xyz/gtmyidkigr.html

[R34] 退出时清理
来源：http://hz.gotoacloud.top/gtwinkyssk.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.quarkkingdee.top/gtzcwrvthm.html

[R35] 后台执行并等待
来源：http://hz.shuidangran.top/gtwgkzbpci.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.xingfuxueyuan.xyz/gtevupogcf.html

[R36] 并发执行多个任务
来源：http://hz.hnqzz.top/gtuadvlxon.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jlsjyb.cn/gthawghwjm.html

[R37] 把输出赋给变量
来源：http://hz.kuanghao11.cn/gtnzerpwwc.html

files=$(ls -1)
来源：http://hz.hongshengwenyu.top/gtyhxomxpz.html

[R38] 管道串联
来源：http://hz.iojbl.cn/gtijkmkdoz.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jianghu66.top/gtgwzifdmn.html

[R39] 重定向标准输出与错误
来源：http://hz.pycfn.com/gtmdzeujdy.html

cmd > out.log 2>&1
来源：http://hz.yvedp.cn/gtfmeokmya.html

[R40] 追加写日志
来源：http://hz.meibo888.top/gtcttsfdbf.html

echo "log" >> out.log
来源：http://hz.hammf.cn/gtaluqvnlq.html

[R41] 丢弃输出
来源：http://hz.andypj.xyz/gtjlcothmj.html

cmd >/dev/null 2>&1
来源：http://hz.smart0.xyz/gtjdoowgjk.html

[R42] 输入重定向
来源：http://hz.sysykeji.top/gtxntrdnng.html

wc -l < a.txt
来源：http://hz.yj202588.top/gtyfyaypkb.html

[R43] 按名字查找文件
来源：http://hz.havefunace.top/gttvvwwvrx.html

find . -name "*.log" -type f
来源：http://hz.jqgufenzy.top/gtogkxigvk.html

[R44] 按修改时间查找
来源：http://hz.shzxlz.cn/gtdavqlkkk.html

find . -mtime -7 -type f
来源：http://hz.chenjidiqi.icu/gtbboiadcn.html

[R45] 批量删除
来源：http://hz.ppjwa.cn/gtsqnqrwpo.html

find . -name "*.tmp" -delete
来源：http://hz.shanyushiyangtech.top/gtelhardol.html

[R46] 递归替换文件内容
来源：http://hz.chenzaomai.com/gthuhcqcla.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.c1oappe.top/gtkfgajmrp.html

[R47] sed 单行替换
来源：http://hz.dashuyun.cn/gtfkoaevqr.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yj20258.top/gtojvypyfp.html

[R48] awk 取指定列
来源：http://hz.jinqigufen.top/gteollatzz.html

awk '{print $1, $3}' a.txt
来源：http://hz.zhoulong.xyz/gtmecarwpp.html

[R49] awk 带条件
来源：http://hz.ehwqpu.com/gtaywuwbxk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.aizwys.cn/gtmcxosazz.html

[R50] awk 求和
来源：http://hz.ywan-chungtsiang.top/gtokmovdov.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yvedp.cn/gtukcsmmpw.html

[R51] 排序去重取前几
来源：http://hz.tanke756.top/gtbgnjuwlx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.zhiwuduotai.top/gtwuppiqvy.html

[R52] 统计行数
来源：http://hz.jinyuanbaomall.cn/gtqpoxjgqa.html

wc -l a.txt
来源：http://hz.jyoumei.cn/gtafnoybbh.html

[R53] 查看文件头与实时尾
来源：http://hz.xziqi.cn/gtqkqibenu.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.andypj.xyz/gtkqmwusyr.html

[R54] 比较两个文件
来源：http://hz.pengpengdd.cyou/gtrluajnau.html

diff a.txt b.txt
来源：http://hz.yuanzhike.top/gtzbfewxzv.html

[R55] 压缩与解压
来源：http://hz.yj20258.top/gtvykgkhrh.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yangfankeji.com/gtpshwjoiw.html

[R56] 远程拷贝
来源：http://hz.yanxiufei.cn/gtfhbdwmbh.html

scp file user@host:/path/
来源：http://hz.zhiwuduotai.top/gtqzornxwf.html

[R57] 远程执行命令
来源：http://hz.iojbl.cn/gtfvoatggh.html

ssh user@host 'uptime'
来源：http://hz.hywenlv.cn/gtqegoowrm.html

[R58] 下载文件
来源：http://hz.jyoumei.cn/gtuslbllcn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.zhixingplan.top/gteirzgrqj.html

[R59] 发 POST JSON
来源：http://hz.smart0.xyz/gtebxzrzcz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.kuanghao11.cn/gtzaiwpwrf.html

[R60] 只看 HTTP 状态码
来源：http://hz.hnqzz.top/gtniduhtrc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.hywenlv.cn/gtbcywiczh.html

[R61] 磁盘占用
来源：http://hz.hysaishi.cn/gtlormmbcx.html

df -h;  du -sh *
来源：http://hz.xinyue.icu/gtvlnahohr.html

[R62] 找最占空间的文件
来源：http://hz.aizwys.cn/gthlvdnyit.html

du -ah . | sort -rh | head -10
来源：http://hz.mhx1999.top/gtzvnqqske.html

[R63] 内存与进程
来源：http://hz.wangshuangyany.cn/gtjnvaccai.html

free -h;  ps aux | grep nginx
来源：http://hz.shangyingyoupin.top/gtbeajoaih.html

[R64] 结束进程
来源：http://hz.xinyue.icu/gtmgxfbqop.html

kill -9 $(pgrep -f app.py)
来源：http://hz.zycfv.cn/gtehndgetn.html

[R65] 查看端口占用
来源：http://hz.gogol.net.cn/gtolniscqx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.tian-w.cn/gtofozndzd.html

[R66] 定时任务
来源：http://hz.aizwys.cn/gtyxzczyrw.html

crontab -e;  crontab -l
来源：http://hz.nanxuanxn.top/gtjrwnzjvx.html

[R67] 生成随机十六进制串
来源：http://hz.cucudq.cn/gtrpaoxwkw.html

openssl rand -hex 16
来源：http://hz.yueranfly.top/gtfnjhpvsg.html

[R68] 计算文件校验值
来源：http://hz.jinyuanbaomall.cn/gtzssrcvub.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.jqgfzy.top/gtiqptffxl.html

[R69] 生成随机密码
来源：http://hz.daria6918.cn/gthmbcrnqk.html

head -c 16 /dev/urandom | base64
来源：http://hz.ehwqpu.com/gtueawfoka.html

[R70] 时间戳与互转
来源：http://hz.birdmap.top/gtbcmrfabu.html

date +%s;  date -d @1700000000
来源：http://hz.dashuyun.cn/gtucmnxoty.html

[R71] 日期格式化
来源：http://hz.daria6918.cn/gtmabeuexz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.tian-w.cn/gtpgbainjz.html

[R72] 等待端口就绪
来源：http://hz.jiagoushi.top/gtklvbxczw.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.feifeiyinyue.top/gtywhpzlkk.html

[R73] 分割大日志
来源：http://hz.ybcxt.top/gtpmfvhbjc.html

split -l 1000 big.log part_
来源：http://hz.zhixingplan.top/gtqhoxnxpy.html

[R74] 批量重命名
来源：http://hz.wangshuangyany.cn/gtdxrroqel.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.hnxiangtu.top/gttiwqjciu.html

[R75] 导出环境变量
来源：http://hz.shanyushiyangtech.top/gtwmbnlgem.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.cheryme.top/gtkmlvdxma.html

[R76] 使用临时文件
来源：http://hz.yvedp.cn/gtjudvnjmr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.hysaishi.cn/gtaajhxxyh.html

[R77] 读取用户输入
来源：http://hz.shangyingyoupin.top/gtspnlekdq.html

read -rp "请输入: " ans
来源：http://hz.xuetiantiany.cn/gtidhyjnio.html

[R78] 交互式菜单
来源：http://hz.pycfn.com/gttkiobzin.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.gzhubu.top/gtcnkoiyjr.html

[R79] 解析命令行选项
来源：http://hz.jinqigfzy.top/gtmsqsmigg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.cqqwz.cn/gtdrvywtzb.html

[R80] 查看脚本执行耗时
来源：http://hz.meibo888.top/gtajngufwr.html

time ./run.sh
来源：http://hz.xuetiantiany.cn/gtpctrggei.html

================================================================================
来源：http://hz.yanxiufei.cn/gtmuivnpbp.html

S. C / C++ 专题
来源：http://hz.birdmap.top/gtmbvmtnvq.html

================================================================================
来源：http://hz.hnxiangtu.top/gtandkmfbl.html

[S01] C：Hello World
来源：http://hz.yuxming.cn/gttpsfcwqg.html

#include <stdio.h>
来源：http://hz.316326.xyz/gtkkazfuxs.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yj202588.top/gttoxmywvv.html

[S02] C：变量与格式化输出
来源：http://hz.jiagoushi.top/gteanlqzac.html

int a = 10; printf("%d\n", a);
来源：http://hz.yj20258.top/gtkslnrluk.html

[S03] C：读入整数
来源：http://hz.gogol.net.cn/gtzzjxxmdl.html

int x; scanf("%d", &x);
来源：http://hz.zycfv.cn/gtfpesdtyc.html

[S04] C：字符串复制
来源：http://hz.c1oappe.top/gtektcvuqq.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.aibaodan.cn/gtrpgxqdlv.html

[S05] C：字符串长度
来源：http://hz.bjfxy.top/gtqqcdtfkw.html

strlen(s)
来源：http://hz.sufxvd.cn/gtuiefqyit.html

[S06] C：字符串比较
来源：http://hz.guannengcc.top/gtucaukxbp.html

strcmp(a, b) == 0
来源：http://hz.snrcjt.cn/gtmmtexybl.html

[S07] C：数组遍历求和
来源：http://hz.shzxlz.cn/gtikkmdpfv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.hongshengwenyu.top/gteirlkopz.html

[S08] C：动态内存分配与释放
来源：http://hz.hnxiangtu.top/gtqhvnzyix.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.nwbrower.top/gtxabpktjc.html

[S09] C：结构体定义与初始化
来源：http://hz.dianchejie.cn/gteutxaoaq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.chenlongwang.top/gtfoqmjblg.html

[S10] C：指针与解引用
来源：http://hz.hongshengwenyu.top/gtinfjngee.html

int *p = &a;  *p = 5;
来源：http://hz.tian-w.cn/gthcaarcxb.html

[S11] C：逐行读文件
来源：http://hz.mhx1999.top/gtlnboneix.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.fengsongda.top/gthxmmhhlv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.xuanzx.com/gtdksemxmq.html

fclose(f);
来源：http://hz.yvedp.cn/gtenfloibr.html

[S12] C：写文件
来源：http://hz.zhixingplan.top/gtgayvsipc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.pengpengdd.cyou/gtnrrltirt.html

[S13] C：宏定义
来源：http://hz.xuanzx.com/gtlofnmjld.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.pengpengdd.cyou/gtvrxykwcr.html

[S14] C：枚举
来源：http://hz.jinqigufen.top/gtqwhxcjmc.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.aibaodan.cn/gtqvkungvh.html

[S15] C：类型转换
来源：http://hz.jiagoushi.top/gtsqrhnvzl.html

(double) a / b
来源：http://hz.hywenlv.cn/gtqpmncoky.html

[S16] C：位操作置位
来源：http://hz.fengsongda.top/gtkaagqagv.html

x |= (1 << 3);
来源：http://hz.aibaodan.cn/gtyheghjuv.html

[S17] C：安全拼接字符串
来源：http://hz.aibaodan.cn/gtudhgoqvm.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.52xcode.cn/gtqjpribxg.html

[S18] C：命令行参数
来源：http://hz.yuxming.cn/gtkknsprlc.html

int main(int argc, char **argv)
来源：http://hz.zdqjudy.top/gthpsjkycc.html

[S19] C：快速排序
来源：http://hz.zhijiandao.cn/gtpqycalsf.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.tian-w.cn/gtdigsdyhn.html

[S20] C：二分查找
来源：http://hz.yj202588.top/gtzuvjvpsu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.shangyingyoupin.top/gtsvwvthxm.html

[S21] C：字符类别判断
来源：http://hz.tian-w.cn/gtzgvavkwg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.snrcjt.cn/gtglpjbzss.html

[S22] C：字符串转数字
来源：http://hz.dianchejie.cn/gtyldpimwz.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.shangyingyoupin.top/gtpnvwoaps.html

[S23] C：随机数
来源：http://hz.birdmap.top/gtniolrfls.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.hywenlv.cn/gtzjlezihw.html

[S24] C：获取本地时间
来源：http://hz.wangdashe.top/gtufyrvfui.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.sxryk.cn/gtmlcqizbi.html

[S25] C：内存拷贝
来源：http://hz.havefunace.top/gttaktkpqk.html

memcpy(dst, src, n);
来源：http://hz.fengsongda.top/gtyolgrwpk.html

[S26] C：内存清零
来源：http://hz.guowangkeji.top/gtulwrxzeq.html

memset(a, 0, sizeof a);
来源：http://hz.ywan-chungtsiang.top/gtsaruneyb.html

[S27] C：定义常量
来源：http://hz.xinyue.icu/gtcttffszv.html

const double PI = 3.14159;
来源：http://hz.smart0.xyz/gtfezyhgod.html

[S28] C：静态变量
来源：http://hz.gzhubu.top/gthifqqdmz.html

static int counter = 0;
来源：http://hz.shzxlz.cn/gtcyfoisrq.html

[S29] C：变参函数
来源：http://hz.gaohongyu789.top/gtptjhicsl.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.sxryk.cn/gtrmrlhcwm.html

[S30] C：头文件保护
来源：http://hz.sufxvd.cn/gtnrmvgzbv.html

#ifndef X_H
来源：http://hz.yangfankeji.com/gtvfiwqdgj.html

#define X_H
来源：http://hz.meibo888.top/gtuxujhhzo.html

#endif
来源：http://hz.iojbl.cn/gtrhxotbcy.html

[S31] C++：Hello World
来源：http://hz.haohaochexian.top/gtdvbuwfer.html

#include <iostream>
来源：http://hz.yongpay.top/gttrcilqth.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.svipenyu.cn/gtrpmpuhkm.html

[S32] C++：字符串
来源：http://hz.xuanzx.com/gtzdmopwmj.html

std::string s = "hi";  s += "!";
来源：http://hz.zhoulong.xyz/gtevjmhifh.html

[S33] C++：vector 增删
来源：http://hz.guannengcc.top/gtmdxxcjcd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.shangyingyoupin.top/gtcopyzqgb.html

[S34] C++：遍历 vector
来源：http://hz.yongpay.top/gtcctbockq.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.hammf.cn/gtxhaxngyn.html

[S35] C++：map
来源：http://hz.yj202588.top/gttywmmqmm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hysaishi.cn/gtxerzmews.html

[S36] C++：unordered_map
来源：http://hz.jinyuanbaomall.cn/gtfgnaowoy.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.snrcjt.cn/gtbfnkptae.html

[S37] C++：set
来源：http://hz.guannengcc.top/gtswusptye.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.svipenyu.cn/gtygtaqmel.html

[S38] C++：排序
来源：http://hz.ydjk.org.cn/gtnfbyfqhk.html

std::sort(v.begin(), v.end());
来源：http://hz.zhixingplan.top/gtyybqclvo.html

[S39] C++：自定义比较器排序
来源：http://hz.gogol.net.cn/gtwfglgafj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.fengsongda.top/gtfwrhewhw.html

[S40] C++：查找元素
来源：http://hz.9152youxi.cn/gtiwxvpeal.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.cqqwz.cn/gtozhcwwer.html

[S41] C++：类与构造函数
来源：http://hz.52xcode.cn/gtuwytihyr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.zhongyouzk.top/gteauncyrf.html

[S42] C++：继承与虚函数
来源：http://hz.jinghuilouyu.cn/gtjooopmgh.html

class B : public Base { public: void f() override {} };
来源：http://hz.shanyushiyangkeji.top/gtytppcszt.html

[S43] C++：智能指针
来源：http://hz.yuxming.cn/gtszgcslng.html

auto p = std::make_unique<int>(5);
来源：http://hz.yuanzhike.top/gticlinaaf.html

[S44] C++：引用传参
来源：http://hz.daxiang520.top/gtdqjwktue.html

void inc(int &x) { ++x; }
来源：http://hz.gotoacloud.top/gtcahbkwms.html

[S45] C++：lambda
来源：http://hz.hongshengwenyu.top/gtngqrobyw.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.hfpthk.cn/gtyiuexaim.html

[S46] C++：函数模板
来源：http://hz.xingfuxueyuan.xyz/gtdbyaisis.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.iojbl.cn/gtfnwakfuu.html

[S47] C++：结构化绑定遍历
来源：http://hz.jqgfzy.top/gtbchngjie.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.hfpthk.cn/gtfvzuulko.html

[S48] C++：逐行读文件
来源：http://hz.andypj.xyz/gtjdvdzvhr.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.pengpengdd.cyou/gttbhfceic.html


<!-- 参考信息 -->