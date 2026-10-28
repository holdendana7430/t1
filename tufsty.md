代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.guannengcc.top/gtxqalsquj.html

[Q75] 日期格式化
来源：http://hz.xziqi.cn/gtmnchwdbz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.hongshengwenyu.top/gthwjsxuqp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.zhongyouzk.top/gtsjbhttwf.html

[Q76] 按天统计
来源：http://hz.dianchejie.cn/gtfjascdpt.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.zhaomingkeji.xyz/gtyfjsasxq.html

[Q77] 时间加减
来源：http://hz.yuxming.cn/gtindivtlo.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.hongshengwenyu.top/gtfbhciyji.html

[Q78] 当前时间
来源：http://hz.sweek.top/gtdjmulcvy.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.xinyue.icu/gtzxemyzuo.html

[Q79] 字符串拼接
来源：http://hz.cqqwz.cn/gtmjmnvzde.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.hnqzz.top/gttvfwfsng.html

[Q80] 字符串截取
来源：http://hz.shzxlz.cn/gtncxarkmb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jlsjyb.cn/gtnxsdkkvu.html

[Q81] 字符串替换
来源：http://hz.ywan-chungtsiang.top/gtoywvphma.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.ydzc1.top/gtxhwulaof.html

[Q82] 字符长度与字节长度
来源：http://hz.dashuyun.cn/gtyyzdibee.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.52xcode.cn/gtzqcccysf.html

[Q83] 大小写转换
来源：http://hz.hysaishi.cn/gtacxpjcoo.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.tanke756.top/gtkpqkuakc.html

[Q84] 去除首尾空格
来源：http://hz.haohaochexian.top/gtaoqeysec.html

SELECT TRIM(name) FROM users;
来源：http://hz.yj20258888.top/gtjyjsbmso.html

[Q85] 数值取整
来源：http://hz.nwbrower.top/gtbnxyhclo.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.zhengqikj.top/gtdzxbphtx.html

[Q86] 读取 JSON 字段
来源：http://hz.jinqigufen.top/gtlesxgxgs.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.zhixingplan.top/gtctpgxwaz.html

[Q87] JSON 字段做条件
来源：http://hz.zhijiandao.cn/gtnwlzdcbp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.hywenlv.cn/gtobwqxaws.html

[Q88] 行转列（条件聚合）
来源：http://hz.hywenlv.cn/gtzdgvohlb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.aibaodan.cn/gtoqzbshpf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.xuanzx.com/gtifsbdhfi.html

[Q89] 判断表是否存在
来源：http://hz.wangdashe.top/gthrrxikva.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zdqjudy.top/gtqvepgjth.html

[Q90] 生成序号列
来源：http://hz.jiagoushi.top/gtjlrrzzyk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.hnxiangtu.top/gtbsaxljel.html

================================================================================
来源：http://hz.aibaodan.cn/gtpmowaudr.html

R. Bash 专题
来源：http://hz.nanxuanxn.top/gtfowvnhze.html

================================================================================
来源：http://hz.sysykeji.top/gtzjaumzqk.html

[R01] shebang 与严格模式
来源：http://hz.chenlongwang.top/gtgeasccxd.html

#!/usr/bin/env bash
来源：http://hz.bjfxy.top/gtcrilnmgh.html

set -euo pipefail
来源：http://hz.shanyushiyangtech.top/gtxlyzuyex.html

[R02] 变量赋值与使用
来源：http://hz.yueranfly.top/gtncjseceg.html

name="Tom"; echo "$name"
来源：http://hz.jqgufenzy.top/gtkrrdvtlw.html

[R03] 只读变量
来源：http://hz.yueranfly.top/gttriqppje.html

readonly PI=3.14
来源：http://hz.ybcxt.top/gtbevczyye.html

[R04] 位置参数
来源：http://hz.pengpengdd.cyou/gttdboltel.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.jinyuanbaomall.cn/gtdtpdbqsy.html

[R05] 参数默认值
来源：http://hz.guannengcc.top/gtkglwgzym.html

name="${1:-default}"
来源：http://hz.xziqi.cn/gtpgwhcjxm.html

[R06] 判断命令是否存在
来源：http://hz.zycfv.cn/gtjjpgpszn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.cucudq.cn/gtghmsvtoi.html

[R07] if 判断文件
来源：http://hz.hnqzz.top/gtelxhxpus.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.chenlongwang.top/gtyxvrwxck.html

[R08] 数值比较
来源：http://hz.ehwqpu.com/gtspjsskue.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.ppjwa.cn/gtzulvmbal.html

[R09] 字符串比较
来源：http://hz.gogol.net.cn/gtzuxaaawz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.ppjwa.cn/gttcrqjzlk.html

[R10] 正则匹配
来源：http://hz.tianlin.xyz/gtymvplpgi.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yj202588.top/gtzdknqfkx.html

[R11] case 多分支
来源：http://hz.hongshengwenyu.top/gtxwhdnbyu.html

case "$1" in
来源：http://hz.hnqzz.top/gtrjdwbpzu.html

start) echo "启动" ;;
来源：http://hz.ydzc1.top/gtvlblhxuv.html

stop)  echo "停止" ;;
来源：http://hz.gogol.net.cn/gtgrtiyykw.html

*)     echo "未知命令" ;;
来源：http://hz.zhijiandao.cn/gthqkhdeji.html

esac
来源：http://hz.guowangkeji.top/gtkabbhduo.html

[R12] for 遍历文件
来源：http://hz.birdmap.top/gtrejvrtxa.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yueranfly.top/gtkitsgmur.html

[R13] for 计数循环
来源：http://hz.ydjk.org.cn/gtutwdlsgv.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.gogol.net.cn/gtwcvgfqfo.html

[R14] C 风格 for
来源：http://hz.cashguo.top/gtdbsiowzs.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.xylfe.cn/gttajocsnk.html

[R15] while 逐行读文件
来源：http://hz.meibo888.top/gtohjceffo.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.hfpthk.cn/gtjmtejrjc.html

[R16] until 等待条件
来源：http://hz.tian-w.cn/gtzmekcdtj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.daxiang520.top/gtauewxmax.html

[R17] 数组定义与取值
来源：http://hz.hammf.cn/gtooqwvpid.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.wangshuangyany.cn/gtnzrsrfzk.html

[R18] 遍历数组
来源：http://hz.guannengcc.top/gtxkovilqk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.cucudq.cn/gtestgpvcq.html

[R19] 数组长度
来源：http://hz.nanxinkj.top/gtdelglvel.html

echo "${#arr[@]}"
来源：http://hz.xylfe.cn/gtlcltoabm.html

[R20] 关联数组（字典）
来源：http://hz.guannengcc.top/gtsoeptvyy.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.ywan-chungtsiang.top/gtccvxriou.html

[R21] 字符串长度
来源：http://hz.nanxinkj.top/gtwmmzmfgb.html

echo "${#s}"
来源：http://hz.chenjidiqi.icu/gtuugguikc.html

[R22] 截取子串
来源：http://hz.aizwys.cn/gtqzbtfjyi.html

echo "${s:0:5}"
来源：http://hz.wangdashe.top/gtcugqiryb.html

[R23] 字符串替换
来源：http://hz.jianghu66.top/gtmxnzyquc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.meibo888.top/gtuplaucot.html

[R24] 大小写转换
来源：http://hz.zhixingplan.top/gtzjxonyuu.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.fzhhl.top/gtgockaxdv.html

[R25] 去后缀 / 去前缀
来源：http://hz.bjfxy.top/gtjgzyuqee.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.feifeiyinyue.top/gtdbrsboad.html

[R26] 命令替换
来源：http://hz.9152youxi.cn/gtoqietnco.html

now=$(date +%F); echo "$now"
来源：http://hz.gotoacloud.top/gtnpizmmkm.html

[R27] 算术展开
来源：http://hz.wangdashe.top/gtfaqbnwhc.html

echo $((1 + 2 * 3))
来源：http://hz.hywenlv.cn/gtbwlmaufv.html

[R28] 浮点运算
来源：http://hz.xylfe.cn/gtmlogazrr.html

echo "scale=2; 10/3" | bc
来源：http://hz.ppjwa.cn/gtajddbzrz.html

[R29] 定义函数
来源：http://hz.jinghuilouyu.cn/gtlbwurmaz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.guowangkeji.top/gtmanqfvnv.html

[R30] 函数返回状态码
来源：http://hz.ywan-chungtsiang.top/gtpyyvdxlr.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jinqigufen.top/gtrdzyqzdd.html

[R31] 局部变量
来源：http://hz.yuanzhike.top/gtmarsqjgz.html

f() { local x=1; echo "$x"; }
来源：http://hz.zhijiandao.cn/gterndyutu.html

[R32] 参数个数校验
来源：http://hz.yanxiufei.cn/gtsqsjjrue.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.nwbrower.top/gtkohfhowt.html

[R33] 捕获错误并提示行号
来源：http://hz.zhijiandao.cn/gtrpcpbhyg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.yanxiufei.cn/gtwgaenynt.html

[R34] 退出时清理
来源：http://hz.xziqi.cn/gtsngeqvpc.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.nanxuanxn.top/gtjoxexyvr.html

[R35] 后台执行并等待
来源：http://hz.yuxming.cn/gtwuyyossw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.xingfuxueyuan.xyz/gtitjhfwjm.html

[R36] 并发执行多个任务
来源：http://hz.pycfn.com/gtivttdqgw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.havefunace.top/gtvmotuwtc.html

[R37] 把输出赋给变量
来源：http://hz.sufxvd.cn/gtetqytdpf.html

files=$(ls -1)
来源：http://hz.tanke756.top/gtabgjlvpo.html

[R38] 管道串联
来源：http://hz.fzhhl.top/gtytefndzs.html

cat a.txt | grep -i error | wc -l
来源：http://hz.zycfv.cn/gtkcqitshn.html

[R39] 重定向标准输出与错误
来源：http://hz.daxiang520.top/gtezbxlhjn.html

cmd > out.log 2>&1
来源：http://hz.cashguo.top/gtmjukznsu.html

[R40] 追加写日志
来源：http://hz.yj20258888.top/gtmnnuyuaq.html

echo "log" >> out.log
来源：http://hz.xinyue.icu/gtrudmgmrn.html

[R41] 丢弃输出
来源：http://hz.hfpthk.cn/gtnqpcrkxu.html

cmd >/dev/null 2>&1
来源：http://hz.tianlin.xyz/gtbhmgonrs.html

[R42] 输入重定向
来源：http://hz.tanke756.top/gtmwuyerih.html

wc -l < a.txt
来源：http://hz.xinyue.icu/gtxqldgpcq.html

[R43] 按名字查找文件
来源：http://hz.yanxiufei.cn/gtyqvclehq.html

find . -name "*.log" -type f
来源：http://hz.fengsongda.top/gtvmpujcxo.html

[R44] 按修改时间查找
来源：http://hz.ivvv.top/gtqjrsligk.html

find . -mtime -7 -type f
来源：http://hz.yj202588.top/gtvmzomtkk.html

[R45] 批量删除
来源：http://hz.hongshengwenyu.top/gtxpkpugfn.html

find . -name "*.tmp" -delete
来源：http://hz.pengpengdd.cyou/gtpodmkort.html

[R46] 递归替换文件内容
来源：http://hz.cashguo.top/gtglhpxgdm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.hywenlv.cn/gtxdycvxtd.html

[R47] sed 单行替换
来源：http://hz.feifeiyinyue.top/gtcxhfaygl.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.wangshuangyany.cn/gtoalhrxsf.html

[R48] awk 取指定列
来源：http://hz.0kj1m.cn/gtrzvukvvc.html

awk '{print $1, $3}' a.txt
来源：http://hz.yj20258888.top/gtcuenfbnn.html

[R49] awk 带条件
来源：http://hz.birdmap.top/gtfbqeiyul.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.xingfuxueyuan.xyz/gtkrkbtllu.html

[R50] awk 求和
来源：http://hz.daxiang520.top/gtieyxdhfq.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.guannengcc.top/gtrkxhbfiq.html

[R51] 排序去重取前几
来源：http://hz.xuanzx.com/gtkfxllzao.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.andypj.xyz/gtsqztyxth.html

[R52] 统计行数
来源：http://hz.ybcxt.top/gtcbbgjtdu.html

wc -l a.txt
来源：http://hz.guowangkeji.top/gttmcrqccn.html

[R53] 查看文件头与实时尾
来源：http://hz.wangdashe.top/gtkgojbbqi.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.meibo888.top/gtiagaqguz.html

[R54] 比较两个文件
来源：http://hz.chenlongwang.top/gtecetjfzk.html

diff a.txt b.txt
来源：http://hz.cheryme.top/gtcaabazgw.html

[R55] 压缩与解压
来源：http://hz.pycfn.com/gtyoreahgl.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yj202588.top/gtpouklkbh.html

[R56] 远程拷贝
来源：http://hz.iojbl.cn/gtewqybsyi.html

scp file user@host:/path/
来源：http://hz.xingfuxueyuan.xyz/gtawvdfrkr.html

[R57] 远程执行命令
来源：http://hz.fengsongda.top/gtqcfhgtwl.html

ssh user@host 'uptime'
来源：http://hz.iojbl.cn/gtboxcsiwi.html

[R58] 下载文件
来源：http://hz.mhx1999.top/gtbrpamocq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.daria6918.cn/gtdmjiypna.html

[R59] 发 POST JSON
来源：http://hz.haohaochexian.top/gttekggspf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.havefunace.top/gtnkncxxcj.html

[R60] 只看 HTTP 状态码
来源：http://hz.tianlin.xyz/gtnwwikiwn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.cdnleiting.top/gtlhttywjc.html

[R61] 磁盘占用
来源：http://hz.gotoacloud.top/gthjeplazh.html

df -h;  du -sh *
来源：http://hz.yj202588.top/gtylqvvvbt.html

[R62] 找最占空间的文件
来源：http://hz.xingfuxueyuan.xyz/gtctwnnxqb.html

du -ah . | sort -rh | head -10
来源：http://hz.hnxiangtu.top/gtniplwqab.html

[R63] 内存与进程
来源：http://hz.feifeiyinyue.top/gtiiwiaboi.html

free -h;  ps aux | grep nginx
来源：http://hz.shangyingyoupin.top/gtgvftywkq.html

[R64] 结束进程
来源：http://hz.jlsjyb.cn/gttaqvpiqr.html

kill -9 $(pgrep -f app.py)
来源：http://hz.hongshengwenyu.top/gtjeupponi.html

[R65] 查看端口占用
来源：http://hz.guowangkeji.top/gtbdjrovvi.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.ivvv.top/gtyxqgdkfl.html

[R66] 定时任务
来源：http://hz.sxryk.cn/gtkyolxraj.html

crontab -e;  crontab -l
来源：http://hz.kuanghao11.cn/gtcuwxdlap.html

[R67] 生成随机十六进制串
来源：http://hz.cashguo.top/gtmifxgfkx.html

openssl rand -hex 16
来源：http://hz.guowangkeji.top/gtrsiecoyo.html

[R68] 计算文件校验值
来源：http://hz.yvedp.cn/gtzdiysukm.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.52xcode.cn/gttkhofvdr.html

[R69] 生成随机密码
来源：http://hz.dashuyun.cn/gtrwxvqlmb.html

head -c 16 /dev/urandom | base64
来源：http://hz.ydzc1.top/gtkrvtkvhl.html

[R70] 时间戳与互转
来源：http://hz.jinqigufen.top/gtjvmzakec.html

date +%s;  date -d @1700000000
来源：http://hz.meibo888.top/gtsnwfttkf.html

[R71] 日期格式化
来源：http://hz.yangfankeji.com/gtgzdnvbpz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jqgufenzy.top/gtrtbobkbx.html

[R72] 等待端口就绪
来源：http://hz.jinghuilouyu.cn/gtpshkwymx.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.pengpengdd.cyou/gtlmnnsegd.html

[R73] 分割大日志
来源：http://hz.jinqigfzy.top/gtwfqzgjts.html

split -l 1000 big.log part_
来源：http://hz.cdnleiting.top/gtgrzzvarx.html

[R74] 批量重命名
来源：http://hz.chenjidiqi.icu/gtkbpdybtz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.pycfn.com/gttazwvxle.html

[R75] 导出环境变量
来源：http://hz.pycfn.com/gtqudmknxx.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.gogol.net.cn/gtttcfeauy.html

[R76] 使用临时文件
来源：http://hz.hnxiangtu.top/gticpsnhfs.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.haohaochexian.top/gtfgaslrsl.html

[R77] 读取用户输入
来源：http://hz.jyoumei.cn/gtzlxfeimx.html

read -rp "请输入: " ans
来源：http://hz.birdmap.top/gtbmxftbpb.html

[R78] 交互式菜单
来源：http://hz.yangfankeji.com/gttbhnibzu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.sweek.top/gtoepoyado.html

[R79] 解析命令行选项
来源：http://hz.andypj.xyz/gtdjfgivbm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.sysykeji.top/gtodhathcg.html

[R80] 查看脚本执行耗时
来源：http://hz.cqqwz.cn/gtdieujvot.html

time ./run.sh
来源：http://hz.yj20258888.top/gtgbhirzny.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtgwfaidsq.html

S. C / C++ 专题
来源：http://hz.svipenyu.cn/gthfqlruqm.html

================================================================================
来源：http://hz.haohaochexian.top/gtfvircmpg.html

[S01] C：Hello World
来源：http://hz.nwbrower.top/gtphcellkc.html

#include <stdio.h>
来源：http://hz.yj202588.top/gthyexekee.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.bjfxy.top/gtgncvfqql.html

[S02] C：变量与格式化输出
来源：http://hz.yj20258.top/gtenjfvpbp.html

int a = 10; printf("%d\n", a);
来源：http://hz.yonumen.top/gthownzpma.html

[S03] C：读入整数
来源：http://hz.birdmap.top/gtmpvwohto.html

int x; scanf("%d", &x);
来源：http://hz.pengpengdd.cyou/gtxsyiezky.html

[S04] C：字符串复制
来源：http://hz.jqgufenzy.top/gtjjiomnrr.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.cdnleiting.top/gtxnmbjxqd.html

[S05] C：字符串长度
来源：http://hz.sxryk.cn/gtxaiphbiu.html

strlen(s)
来源：http://hz.gzhubu.top/gtvcynrcvo.html

[S06] C：字符串比较
来源：http://hz.yueranfly.top/gtoghitgay.html

strcmp(a, b) == 0
来源：http://hz.vqdsnc.cn/gtauitffso.html

[S07] C：数组遍历求和
来源：http://hz.redwolf501.top/gtzpqkxioq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.shanyushiyangkeji.top/gtsewtooiq.html

[S08] C：动态内存分配与释放
来源：http://hz.wangdashe.top/gtseywdfbk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.hnxiangtu.top/gtjpmhzmtb.html

[S09] C：结构体定义与初始化
来源：http://hz.pengpengdd.cyou/gtdtgpbmgr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.gogol.net.cn/gtmfgwzpej.html

[S10] C：指针与解引用
来源：http://hz.jyoumei.cn/gturnvavwy.html

int *p = &a;  *p = 5;
来源：http://hz.shzxlz.cn/gthhjwhkqs.html

[S11] C：逐行读文件
来源：http://hz.fzhhl.top/gtvzkenlct.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.hywenlv.cn/gtgrjbxbgx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.vqdsnc.cn/gtvxufagie.html

fclose(f);
来源：http://hz.cucudq.cn/gtdyqszxno.html

[S12] C：写文件
来源：http://hz.snrcjt.cn/gtycgmruwc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.cucudq.cn/gtndzmpoxf.html

[S13] C：宏定义
来源：http://hz.c1oappe.top/gtwewiddrh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.chenzaomai.com/gthmapyqpf.html

[S14] C：枚举
来源：http://hz.ppjwa.cn/gtzanhupks.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.xziqi.cn/gtgkujkrjz.html

[S15] C：类型转换
来源：http://hz.yueranfly.top/gthrhotigm.html

(double) a / b
来源：http://hz.yvedp.cn/gtvhawxyxp.html

[S16] C：位操作置位
来源：http://hz.jinghuilouyu.cn/gtzzdaxwdk.html

x |= (1 << 3);
来源：http://hz.daxiang520.top/gtgdnibcvp.html

[S17] C：安全拼接字符串
来源：http://hz.guannengcc.top/gtgnojshlk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.smart0.xyz/gtpidlysvw.html

[S18] C：命令行参数
来源：http://hz.52xcode.cn/gtbxnvotby.html

int main(int argc, char **argv)
来源：http://hz.c1oappe.top/gtezvekerx.html

[S19] C：快速排序
来源：http://hz.yonumen.top/gtgfiluvmc.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yuxming.cn/gtiypfyzaq.html

[S20] C：二分查找
来源：http://hz.shanyushiyangtech.top/gtdiycnmpg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zycfv.cn/gtrdessdlr.html

[S21] C：字符类别判断
来源：http://hz.daxiang520.top/gtzidjiuke.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.zhijiandao.cn/gtiixtarjz.html

[S22] C：字符串转数字
来源：http://hz.haohaochexian.top/gtozcrljyu.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.iojbl.cn/gtlqvxolzw.html

[S23] C：随机数
来源：http://hz.xingfuxueyuan.xyz/gtxjaitktf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.iojbl.cn/gthzpyfxmy.html

[S24] C：获取本地时间
来源：http://hz.shanyushiyangkeji.top/gtyupywnni.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yvedp.cn/gttozipkjx.html

[S25] C：内存拷贝
来源：http://hz.jiagoushi.top/gtseaefwzi.html

memcpy(dst, src, n);
来源：http://hz.havefunace.top/gthfswrypg.html

[S26] C：内存清零
来源：http://hz.yongpay.top/gtkwzrfajp.html

memset(a, 0, sizeof a);
来源：http://hz.pengpengdd.cyou/gtjjywifxu.html

[S27] C：定义常量
来源：http://hz.sysykeji.top/gtafnitsdd.html

const double PI = 3.14159;
来源：http://hz.wangdashe.top/gtqxpvrhwo.html

[S28] C：静态变量
来源：http://hz.ybcxt.top/gtikzbzsjq.html

static int counter = 0;
来源：http://hz.52xcode.cn/gtvulaqzbe.html

[S29] C：变参函数
来源：http://hz.zhijiandao.cn/gtsvwpevjs.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.havefunace.top/gtevjvpxra.html

[S30] C：头文件保护
来源：http://hz.hywenlv.cn/gtgkbaalzl.html

#ifndef X_H
来源：http://hz.ydjk.org.cn/gteoyheasl.html

#define X_H
来源：http://hz.yj20258888.top/gthqmyyfbp.html

#endif
来源：http://hz.andypj.xyz/gtprkzqgsh.html

[S31] C++：Hello World
来源：http://hz.ydjk.org.cn/gtdcvobifc.html

#include <iostream>
来源：http://hz.guowangkeji.top/gtmlqjnanz.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yuxming.cn/gtpxsdmyaq.html

[S32] C++：字符串
来源：http://hz.yueranfly.top/gtfqjphupn.html

std::string s = "hi";  s += "!";
来源：http://hz.ydzc1.top/gtwippuvph.html

[S33] C++：vector 增删
来源：http://hz.pycfn.com/gtklfjzypc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.chenjidiqi.icu/gtozwmnnob.html

[S34] C++：遍历 vector
来源：http://hz.guowangkeji.top/gtxrusqegw.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.jyoumei.cn/gtkyuoasgn.html

[S35] C++：map
来源：http://hz.xziqi.cn/gtmcwqmzyp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.chenlongwang.top/gtnbzuopje.html

[S36] C++：unordered_map
来源：http://hz.dianchejie.cn/gtxhuwztkw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ivvv.top/gtdbahpayt.html

[S37] C++：set
来源：http://hz.dashuyun.cn/gtkvbuwudj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.c1oappe.top/gtmswclfsm.html

[S38] C++：排序
来源：http://hz.hywenlv.cn/gtcrnbohhd.html

std::sort(v.begin(), v.end());
来源：http://hz.hnqzz.top/gtinfbtgge.html

[S39] C++：自定义比较器排序
来源：http://hz.quarkkingdee.top/gtawdliasy.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.fzhhl.top/gthrunqzxl.html

[S40] C++：查找元素
来源：http://hz.xuetiantiany.cn/gtuiuzkcip.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.tianlin.xyz/gtkxhiknbq.html

[S41] C++：类与构造函数
来源：http://hz.sufxvd.cn/gtqwqhgnfy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.shanyushiyangkeji.top/gtafayzxql.html

[S42] C++：继承与虚函数
来源：http://hz.tianlin.xyz/gtrsaldael.html

class B : public Base { public: void f() override {} };
来源：http://hz.ivvv.top/gtollnrpoz.html

[S43] C++：智能指针
来源：http://hz.gaohongyu789.top/gtmaocjlry.html

auto p = std::make_unique<int>(5);
来源：http://hz.svipenyu.cn/gtuvwgzmin.html

[S44] C++：引用传参
来源：http://hz.shzxlz.cn/gtasykrtvi.html

void inc(int &x) { ++x; }
来源：http://hz.birdmap.top/gtoxvyhuwy.html


<!-- 参考信息 -->