代发 wailian999

[Q78] 当前时间
来源：http://hz.wangdashe.top/gtgdaxhfcd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.0kj1m.cn/gtwrvwestb.html

[Q79] 字符串拼接
来源：http://hz.wangshuangyany.cn/gtwyhjeiza.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yueranfly.top/gtuyymckxn.html

[Q80] 字符串截取
来源：http://hz.zhoulong.xyz/gtunrfrksh.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.pengpengdd.cyou/gtevohvmwg.html

[Q81] 字符串替换
来源：http://hz.yvedp.cn/gtapaivqyf.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.52xcode.cn/gtpailtaze.html

[Q82] 字符长度与字节长度
来源：http://hz.chenlongwang.top/gtevhastrw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.hywenlv.cn/gtwdazzojg.html

[Q83] 大小写转换
来源：http://hz.zycfv.cn/gtnonbndok.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.zhoulong.xyz/gtzswvzlzf.html

[Q84] 去除首尾空格
来源：http://hz.jiagoushi.top/gtlutaotbq.html

SELECT TRIM(name) FROM users;
来源：http://hz.jinqigfzy.top/gtqatgglzw.html

[Q85] 数值取整
来源：http://hz.yongpay.top/gtpqwhbmil.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.guowangkeji.top/gtrcjpelca.html

[Q86] 读取 JSON 字段
来源：http://hz.yj202588.top/gtyfwvhaxk.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.redwolf501.top/gtwpvszvwe.html

[Q87] JSON 字段做条件
来源：http://hz.xylfe.cn/gtodiaoclo.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.yongpay.top/gtivwupknq.html

[Q88] 行转列（条件聚合）
来源：http://hz.sysykeji.top/gtowhivzqm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yueranfly.top/gtxqnqhtmk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.0kj1m.cn/gtboveaxio.html

[Q89] 判断表是否存在
来源：http://hz.shanyushiyangkeji.top/gtpwmmycua.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.ybcxt.top/gtittxsvtf.html

[Q90] 生成序号列
来源：http://hz.gaohongyu789.top/gtlangsohq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.jiagoushi.top/gtwecbiduw.html

================================================================================
来源：http://hz.tianlin.xyz/gtzdforjit.html

R. Bash 专题
来源：http://hz.zhijiandao.cn/gtwywycwvk.html

================================================================================
来源：http://hz.meibo888.top/gtecuxjgty.html

[R01] shebang 与严格模式
来源：http://hz.havefunace.top/gttflvqbco.html

#!/usr/bin/env bash
来源：http://hz.jinqigufen.top/gtjitqnojm.html

set -euo pipefail
来源：http://hz.daria6918.cn/gtwjibtkxv.html

[R02] 变量赋值与使用
来源：http://hz.pengpengdd.cyou/gtjgwvasge.html

name="Tom"; echo "$name"
来源：http://hz.wangshuangyany.cn/gtqruqypbg.html

[R03] 只读变量
来源：http://hz.jqgfzy.top/gtgzieichs.html

readonly PI=3.14
来源：http://hz.shanyushiyangkeji.top/gtaiaifbfs.html

[R04] 位置参数
来源：http://hz.jyoumei.cn/gtzadcnywu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.hnxiangtu.top/gtlpwsfefp.html

[R05] 参数默认值
来源：http://hz.jyoumei.cn/gtbuosnspl.html

name="${1:-default}"
来源：http://hz.hysaishi.cn/gtolgukiui.html

[R06] 判断命令是否存在
来源：http://hz.jyoumei.cn/gtbejuzvkn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jinqigfzy.top/gtwxplqrlg.html

[R07] if 判断文件
来源：http://hz.guowangkeji.top/gtoulewbce.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.sysykeji.top/gtmdxnfqis.html

[R08] 数值比较
来源：http://hz.yj202588.top/gtsdojxhpl.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.cheryme.top/gtqyfsleyb.html

[R09] 字符串比较
来源：http://hz.zhongyouzk.top/gtkdxtawmt.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.chenzaomai.com/gtslwuuupy.html

[R10] 正则匹配
来源：http://hz.chenjidiqi.icu/gtgwlwsmin.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.kuanghao11.cn/gtcklbsjyy.html

[R11] case 多分支
来源：http://hz.jianghu66.top/gtircrrsvi.html

case "$1" in
来源：http://hz.tanke756.top/gtxsaszyno.html

start) echo "启动" ;;
来源：http://hz.cheryme.top/gtsvpmvesw.html

stop)  echo "停止" ;;
来源：http://hz.zhaomingkeji.xyz/gttwjaeotz.html

*)     echo "未知命令" ;;
来源：http://hz.andypj.xyz/gtqhpdwzey.html

esac
来源：http://hz.dianchejie.cn/gtgppbjong.html

[R12] for 遍历文件
来源：http://hz.ydjk.org.cn/gtqmtlfamp.html

for f in *.txt; do echo "$f"; done
来源：http://hz.chenlongwang.top/gtyowqvxuy.html

[R13] for 计数循环
来源：http://hz.yj20258888.top/gtmbvafppk.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ydzc1.top/gtqhdltcdz.html

[R14] C 风格 for
来源：http://hz.jinqigfzy.top/gtoamigddu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.316326.xyz/gtwufsrxog.html

[R15] while 逐行读文件
来源：http://hz.tianlin.xyz/gtuwipwdme.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.sufxvd.cn/gtikonuxnb.html

[R16] until 等待条件
来源：http://hz.hysaishi.cn/gthqtfusfg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.c1oappe.top/gtcggvstnf.html

[R17] 数组定义与取值
来源：http://hz.xuanzx.com/gtnmcmewtd.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.nanxuanxn.top/gtqkqxwsga.html

[R18] 遍历数组
来源：http://hz.chenzaomai.com/gttznlxytr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.hysaishi.cn/gtphtnsrna.html

[R19] 数组长度
来源：http://hz.c1oappe.top/gtisuphzfo.html

echo "${#arr[@]}"
来源：http://hz.zhongyouzk.top/gtykixlmpy.html

[R20] 关联数组（字典）
来源：http://hz.birdmap.top/gtscxbgusq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.nanxinkj.top/gtljhvzlsw.html

[R21] 字符串长度
来源：http://hz.mhx1999.top/gtnqhtwpix.html

echo "${#s}"
来源：http://hz.sufxvd.cn/gtmbmnpozt.html

[R22] 截取子串
来源：http://hz.ivvv.top/gtyzmunnnd.html

echo "${s:0:5}"
来源：http://hz.gogol.net.cn/gtqgfmzhbe.html

[R23] 字符串替换
来源：http://hz.mhx1999.top/gtjgjtxjhh.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.hongshengwenyu.top/gtwbzxggch.html

[R24] 大小写转换
来源：http://hz.hywenlv.cn/gtgbwbfrsa.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.bjfxy.top/gttngukftv.html

[R25] 去后缀 / 去前缀
来源：http://hz.chenjidiqi.icu/gtbibmyfow.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yuanzhike.top/gtyjlggubd.html

[R26] 命令替换
来源：http://hz.sysykeji.top/gtebgffjxz.html

now=$(date +%F); echo "$now"
来源：http://hz.chenzaomai.com/gtxtppgkom.html

[R27] 算术展开
来源：http://hz.bjfxy.top/gtmqaexvdc.html

echo $((1 + 2 * 3))
来源：http://hz.shanyushiyangtech.top/gteisjyngg.html

[R28] 浮点运算
来源：http://hz.quarkkingdee.top/gtqazsiyit.html

echo "scale=2; 10/3" | bc
来源：http://hz.ppjwa.cn/gtkuvidhvf.html

[R29] 定义函数
来源：http://hz.gotoacloud.top/gtzsbvgfpu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.tanke756.top/gtbjwaxmiw.html

[R30] 函数返回状态码
来源：http://hz.yvedp.cn/gtmpwnbgbm.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.shanyushiyangtech.top/gtsfxxqswy.html

[R31] 局部变量
来源：http://hz.aizwys.cn/gtldjmphrs.html

f() { local x=1; echo "$x"; }
来源：http://hz.vqdsnc.cn/gtbxmvpnex.html

[R32] 参数个数校验
来源：http://hz.meibo888.top/gtkcrjeinv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.sysykeji.top/gtzddvgqwy.html

[R33] 捕获错误并提示行号
来源：http://hz.jlsjyb.cn/gtxaiaksnb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.cucudq.cn/gtyutowjqm.html

[R34] 退出时清理
来源：http://hz.yongpay.top/gtshjvtbmv.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.hnxiangtu.top/gtyzjafxqt.html

[R35] 后台执行并等待
来源：http://hz.shanyushiyangtech.top/gtmqhwkbnp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yangfankeji.com/gtwjnpuugr.html

[R36] 并发执行多个任务
来源：http://hz.aizwys.cn/gtqdpamtnw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.vqdsnc.cn/gtksmgijep.html

[R37] 把输出赋给变量
来源：http://hz.smart0.xyz/gtjrbzrgxr.html

files=$(ls -1)
来源：http://hz.gaohongyu789.top/gtgstkcwas.html

[R38] 管道串联
来源：http://hz.ehwqpu.com/gtmweylnpf.html

cat a.txt | grep -i error | wc -l
来源：http://hz.birdmap.top/gtvtsszuhy.html

[R39] 重定向标准输出与错误
来源：http://hz.ppjwa.cn/gtjyfesrfn.html

cmd > out.log 2>&1
来源：http://hz.zhongyouzk.top/gtjdxcrmvx.html

[R40] 追加写日志
来源：http://hz.zdqjudy.top/gthrnuboar.html

echo "log" >> out.log
来源：http://hz.cashguo.top/gtuaqppjie.html

[R41] 丢弃输出
来源：http://hz.jinghuilouyu.cn/gtlzzuqyze.html

cmd >/dev/null 2>&1
来源：http://hz.yj20258.top/gtrhhtiill.html

[R42] 输入重定向
来源：http://hz.gzhubu.top/gtvokyerkc.html

wc -l < a.txt
来源：http://hz.zhoulong.xyz/gtnhvpoqws.html

[R43] 按名字查找文件
来源：http://hz.aibaodan.cn/gtygtcxlub.html

find . -name "*.log" -type f
来源：http://hz.daxiang520.top/gtfsixlvrh.html

[R44] 按修改时间查找
来源：http://hz.mhx1999.top/gtiywcgsmz.html

find . -mtime -7 -type f
来源：http://hz.mhx1999.top/gtykmazxzf.html

[R45] 批量删除
来源：http://hz.nanxuanxn.top/gtbsvyyhps.html

find . -name "*.tmp" -delete
来源：http://hz.birdmap.top/gttsqzsare.html

[R46] 递归替换文件内容
来源：http://hz.tanke756.top/gtkpyryreq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.xuanzx.com/gthmtxnuax.html

[R47] sed 单行替换
来源：http://hz.andypj.xyz/gtdiwmigce.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.zhoulong.xyz/gtmyddfmpe.html

[R48] awk 取指定列
来源：http://hz.yj20258.top/gteltvwoph.html

awk '{print $1, $3}' a.txt
来源：http://hz.shanyushiyangkeji.top/gtmpbzggvo.html

[R49] awk 带条件
来源：http://hz.yanxiufei.cn/gttpvpkgtq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.nanxuanxn.top/gtxwjelgim.html

[R50] awk 求和
来源：http://hz.vqdsnc.cn/gtctcwitzi.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.redwolf501.top/gtqfrpmqgf.html

[R51] 排序去重取前几
来源：http://hz.jinqigufen.top/gtcggvrbma.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.cheryme.top/gtooinmnjz.html

[R52] 统计行数
来源：http://hz.svipenyu.cn/gtbfnvayue.html

wc -l a.txt
来源：http://hz.birdmap.top/gtvxarvbps.html

[R53] 查看文件头与实时尾
来源：http://hz.vqdsnc.cn/gtuwmaojfn.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.wangshuangyany.cn/gtngynherp.html

[R54] 比较两个文件
来源：http://hz.jqgufenzy.top/gtmgidfphy.html

diff a.txt b.txt
来源：http://hz.bjfxy.top/gttctqgdbw.html

[R55] 压缩与解压
来源：http://hz.tanke756.top/gtalrxjwxh.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.nanxuanxn.top/gtwmtuemmz.html

[R56] 远程拷贝
来源：http://hz.nanxinkj.top/gtfqtvvesz.html

scp file user@host:/path/
来源：http://hz.ivvv.top/gtletnusya.html

[R57] 远程执行命令
来源：http://hz.xylfe.cn/gtvckrugoh.html

ssh user@host 'uptime'
来源：http://hz.cashguo.top/gtjsucokzm.html

[R58] 下载文件
来源：http://hz.xinyue.icu/gthqswqyiz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.shangyingyoupin.top/gtadmugtdh.html

[R59] 发 POST JSON
来源：http://hz.aizwys.cn/gtuelgibso.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jqgfzy.top/gtlhefenbc.html

[R60] 只看 HTTP 状态码
来源：http://hz.yonumen.top/gtxswtjpqg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.zhiwuduotai.top/gtxlabmoam.html

[R61] 磁盘占用
来源：http://hz.ydzc1.top/gthfgcelbq.html

df -h;  du -sh *
来源：http://hz.wangshuangyany.cn/gtnolbtkgv.html

[R62] 找最占空间的文件
来源：http://hz.316326.xyz/gtejlywkrb.html

du -ah . | sort -rh | head -10
来源：http://hz.gzhubu.top/gtfsffysia.html

[R63] 内存与进程
来源：http://hz.hywenlv.cn/gtgpdkejyl.html

free -h;  ps aux | grep nginx
来源：http://hz.tian-w.cn/gtibvpfrlz.html

[R64] 结束进程
来源：http://hz.c1oappe.top/gtvpitywob.html

kill -9 $(pgrep -f app.py)
来源：http://hz.hammf.cn/gtbprizpxc.html

[R65] 查看端口占用
来源：http://hz.chenzaomai.com/gtsgnlrmxm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.zdqjudy.top/gtipfgdapn.html

[R66] 定时任务
来源：http://hz.bjfxy.top/gthatpmced.html

crontab -e;  crontab -l
来源：http://hz.jinqigufen.top/gtqgnvqatd.html

[R67] 生成随机十六进制串
来源：http://hz.tanke756.top/gtjvoslthj.html

openssl rand -hex 16
来源：http://hz.316326.xyz/gthkqkmekr.html

[R68] 计算文件校验值
来源：http://hz.quarkkingdee.top/gthjmuwbrz.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yanxiufei.cn/gtajvmcruz.html

[R69] 生成随机密码
来源：http://hz.sysykeji.top/gtojutaoxs.html

head -c 16 /dev/urandom | base64
来源：http://hz.gotoacloud.top/gtowbocinv.html

[R70] 时间戳与互转
来源：http://hz.jinqigufen.top/gtrdcgijmv.html

date +%s;  date -d @1700000000
来源：http://hz.wangshuangyany.cn/gtrzcurwdp.html

[R71] 日期格式化
来源：http://hz.yj202588.top/gtgbgkrkpx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.cqqwz.cn/gtsjuyebwx.html

[R72] 等待端口就绪
来源：http://hz.hfpthk.cn/gtebshysat.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.cheryme.top/gtpejabbfi.html

[R73] 分割大日志
来源：http://hz.zhiwuduotai.top/gtitwxwqlt.html

split -l 1000 big.log part_
来源：http://hz.zycfv.cn/gtzsjwsjde.html

[R74] 批量重命名
来源：http://hz.ppjwa.cn/gtugajlfsc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.redwolf501.top/gtyttkdbah.html

[R75] 导出环境变量
来源：http://hz.dashuyun.cn/gtfbthxinn.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.aizwys.cn/gtdqghuuze.html

[R76] 使用临时文件
来源：http://hz.hysaishi.cn/gtjtlflyja.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.shangyingyoupin.top/gtwnqrgoov.html

[R77] 读取用户输入
来源：http://hz.cucudq.cn/gtwovybixk.html

read -rp "请输入: " ans
来源：http://hz.hongshengwenyu.top/gtwonmlbvg.html

[R78] 交互式菜单
来源：http://hz.pengpengdd.cyou/gtgkywsooh.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.kuanghao11.cn/gtuuegpdfa.html

[R79] 解析命令行选项
来源：http://hz.hywenlv.cn/gtqhwxkfpo.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.haohaochexian.top/gtfdhqnmvs.html

[R80] 查看脚本执行耗时
来源：http://hz.xziqi.cn/gtgfpncarz.html

time ./run.sh
来源：http://hz.nanxinkj.top/gtwbomufgq.html

================================================================================
来源：http://hz.xziqi.cn/gtinvggmye.html

S. C / C++ 专题
来源：http://hz.birdmap.top/gtnrklqzec.html

================================================================================
来源：http://hz.zhongyouzk.top/gtweczfjmc.html

[S01] C：Hello World
来源：http://hz.yj20258888.top/gtqybebkac.html

#include <stdio.h>
来源：http://hz.ivvv.top/gtyctqhork.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.hnqzz.top/gtmmrdulbw.html

[S02] C：变量与格式化输出
来源：http://hz.zycfv.cn/gtnyqzqeyj.html

int a = 10; printf("%d\n", a);
来源：http://hz.wangdashe.top/gthcdellgi.html

[S03] C：读入整数
来源：http://hz.kuanghao11.cn/gtmwtzufpl.html

int x; scanf("%d", &x);
来源：http://hz.nwbrower.top/gtnkyhueyt.html

[S04] C：字符串复制
来源：http://hz.jlsjyb.cn/gtshmqddxc.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.c1oappe.top/gtpptpuhmj.html

[S05] C：字符串长度
来源：http://hz.hongshengwenyu.top/gtybnobhtp.html

strlen(s)
来源：http://hz.shuidangran.top/gtnjbvcytw.html

[S06] C：字符串比较
来源：http://hz.hongshengwenyu.top/gtbiclramf.html

strcmp(a, b) == 0
来源：http://hz.xuanzx.com/gtokkfxoeq.html

[S07] C：数组遍历求和
来源：http://hz.chenlongwang.top/gtilqjkpav.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.shzxlz.cn/gtewilhcth.html

[S08] C：动态内存分配与释放
来源：http://hz.pycfn.com/gtqrfwcnwr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yuxming.cn/gtulxlluka.html

[S09] C：结构体定义与初始化
来源：http://hz.xylfe.cn/gtfxpaljao.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.dashuyun.cn/gtawhiwjkp.html

[S10] C：指针与解引用
来源：http://hz.hnxiangtu.top/gtdsradhku.html

int *p = &a;  *p = 5;
来源：http://hz.yangfankeji.com/gtuaxxvtoc.html

[S11] C：逐行读文件
来源：http://hz.gzhubu.top/gttbkbzifn.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.shanyushiyangtech.top/gtwrnzmicn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.xziqi.cn/gtliihkiqc.html

fclose(f);
来源：http://hz.hnqzz.top/gtfypkeeqj.html

[S12] C：写文件
来源：http://hz.yangfankeji.com/gtqcttbwut.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.xuetiantiany.cn/gtfjyhfzsg.html

[S13] C：宏定义
来源：http://hz.yongpay.top/gtcgitzkou.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.pycfn.com/gtngahbimr.html

[S14] C：枚举
来源：http://hz.tanke756.top/gtuyutxoau.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.andypj.xyz/gtzedqaivk.html

[S15] C：类型转换
来源：http://hz.quarkkingdee.top/gthcvtctii.html

(double) a / b
来源：http://hz.zhaomingkeji.xyz/gtorrqwelc.html

[S16] C：位操作置位
来源：http://hz.aizwys.cn/gtzftfrgye.html

x |= (1 << 3);
来源：http://hz.yueranfly.top/gtdiouuhfj.html

[S17] C：安全拼接字符串
来源：http://hz.hnqzz.top/gttfhmatxa.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.xingfuxueyuan.xyz/gtnejrmpne.html

[S18] C：命令行参数
来源：http://hz.ywan-chungtsiang.top/gthoigfxjm.html

int main(int argc, char **argv)
来源：http://hz.mhx1999.top/gtarezjhol.html

[S19] C：快速排序
来源：http://hz.jyoumei.cn/gttywvamrv.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.zhixingplan.top/gtrwanqchf.html

[S20] C：二分查找
来源：http://hz.0kj1m.cn/gtgdwhsnqp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.ybcxt.top/gtmmjqfztv.html

[S21] C：字符类别判断
来源：http://hz.tianlin.xyz/gtyadrngcy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.9152youxi.cn/gtrdecqbkb.html

[S22] C：字符串转数字
来源：http://hz.bjfxy.top/gtsjdewkya.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.ybcxt.top/gtbnjovqlh.html

[S23] C：随机数
来源：http://hz.gogol.net.cn/gtbfwbtdon.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.jinghuilouyu.cn/gttpnatpnx.html

[S24] C：获取本地时间
来源：http://hz.zhaomingkeji.xyz/gtfpjdvxdf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.aizwys.cn/gtzutorrue.html

[S25] C：内存拷贝
来源：http://hz.hnqzz.top/gtepmwmkki.html

memcpy(dst, src, n);
来源：http://hz.zycfv.cn/gtiljvbxab.html

[S26] C：内存清零
来源：http://hz.hongshengwenyu.top/gtztkwrxsr.html

memset(a, 0, sizeof a);
来源：http://hz.zdqjudy.top/gtvsdmqgtv.html

[S27] C：定义常量
来源：http://hz.snrcjt.cn/gtfurzsbva.html

const double PI = 3.14159;
来源：http://hz.zhixingplan.top/gtvtzheinj.html

[S28] C：静态变量
来源：http://hz.aibaodan.cn/gtiulbaqnk.html

static int counter = 0;
来源：http://hz.chenjidiqi.icu/gtfdxoaajs.html

[S29] C：变参函数
来源：http://hz.yj20258888.top/gtrgxsqggq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.gotoacloud.top/gtwkyrwdly.html

[S30] C：头文件保护
来源：http://hz.zhixingplan.top/gtwksrimgo.html

#ifndef X_H
来源：http://hz.zhengqikj.top/gtuznqxtjn.html

#define X_H
来源：http://hz.snrcjt.cn/gtmdiwdrkx.html

#endif
来源：http://hz.fzhhl.top/gtcmszhkjz.html

[S31] C++：Hello World
来源：http://hz.cheryme.top/gttpcexijm.html

#include <iostream>
来源：http://hz.haohaochexian.top/gtkiodwaha.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yj202588.top/gtpzknbwev.html

[S32] C++：字符串
来源：http://hz.hnqzz.top/gtnoengxno.html

std::string s = "hi";  s += "!";
来源：http://hz.hfpthk.cn/gtxsicuice.html

[S33] C++：vector 增删
来源：http://hz.feifeiyinyue.top/gttlukhuug.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.xuanzx.com/gteweelymc.html

[S34] C++：遍历 vector
来源：http://hz.yanxiufei.cn/gtcotfdiyj.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.xuetiantiany.cn/gtbbkaglmu.html

[S35] C++：map
来源：http://hz.ppjwa.cn/gtmjnunxoy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jqgufenzy.top/gtdhrefmnq.html

[S36] C++：unordered_map
来源：http://hz.daria6918.cn/gtcfpwoeli.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.gogol.net.cn/gtozakodou.html

[S37] C++：set
来源：http://hz.ydzc1.top/gtbbzxatod.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.ywan-chungtsiang.top/gtfoeznqkd.html

[S38] C++：排序
来源：http://hz.ppjwa.cn/gtfwdyvjkm.html

std::sort(v.begin(), v.end());
来源：http://hz.jyoumei.cn/gtbzjjycom.html

[S39] C++：自定义比较器排序
来源：http://hz.yuanzhike.top/gtjozqthjb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.9152youxi.cn/gtkkstyyeg.html

[S40] C++：查找元素
来源：http://hz.yj20258888.top/gtxfrhmnyw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.nanxuanxn.top/gtjtepyfvn.html

[S41] C++：类与构造函数
来源：http://hz.zdqjudy.top/gteznxzfge.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.svipenyu.cn/gtjiijbfvb.html

[S42] C++：继承与虚函数
来源：http://hz.fzhhl.top/gtqxaekmab.html

class B : public Base { public: void f() override {} };
来源：http://hz.gaohongyu789.top/gttthkddxi.html

[S43] C++：智能指针
来源：http://hz.xinyue.icu/gtvuaikpzb.html

auto p = std::make_unique<int>(5);
来源：http://hz.aibaodan.cn/gtchsxpato.html

[S44] C++：引用传参
来源：http://hz.9152youxi.cn/gttudnnmzg.html

void inc(int &x) { ++x; }
来源：http://hz.meibo888.top/gtnovxmovf.html

[S45] C++：lambda
来源：http://hz.yanxiufei.cn/gtyjeiqfka.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.zhixingplan.top/gtptsyqtdl.html

[S46] C++：函数模板
来源：http://hz.yj202588.top/gtdxjjiafp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.havefunace.top/gthvfjcqex.html

[S47] C++：结构化绑定遍历
来源：http://hz.haohaochexian.top/gtgohsjgzv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.9152youxi.cn/gtcbimytzu.html

[S48] C++：逐行读文件
来源：http://hz.gzhubu.top/gtkddjzkhp.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.shzxlz.cn/gtdigaeaht.html


<!-- 参考信息 -->