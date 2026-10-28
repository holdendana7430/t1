代发 wailian999

[Q76] 按天统计
来源：http://hz.shzxlz.cn/gtbepduyhz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jinyuanbaomall.cn/gtfnomhqll.html

[Q77] 时间加减
来源：http://hz.cashguo.top/gtrqegmquh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.birdmap.top/gtgggkvjsb.html

[Q78] 当前时间
来源：http://hz.hammf.cn/gtvqzbguia.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.redwolf501.top/gtwtqtccka.html

[Q79] 字符串拼接
来源：http://hz.xuanzx.com/gtkgztseli.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.birdmap.top/gtfqoukyio.html

[Q80] 字符串截取
来源：http://hz.pengpengdd.cyou/gteykgnqww.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jyoumei.cn/gtbpznopcm.html

[Q81] 字符串替换
来源：http://hz.jinghuilouyu.cn/gtmwqavcfc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.yueranfly.top/gthrzqamxj.html

[Q82] 字符长度与字节长度
来源：http://hz.zhiwuduotai.top/gtcdpzeaqr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.tianlin.xyz/gtvbdixkkl.html

[Q83] 大小写转换
来源：http://hz.zhaomingkeji.xyz/gtwjwgfizn.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.hfpthk.cn/gtvppwdtzs.html

[Q84] 去除首尾空格
来源：http://hz.xylfe.cn/gtlgwbqgtj.html

SELECT TRIM(name) FROM users;
来源：http://hz.kuanghao11.cn/gtbfjvrned.html

[Q85] 数值取整
来源：http://hz.wangdashe.top/gtmydufiik.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.zycfv.cn/gthdgmsktd.html

[Q86] 读取 JSON 字段
来源：http://hz.birdmap.top/gtefiytnkp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yj20258888.top/gtxmdbdcrz.html

[Q87] JSON 字段做条件
来源：http://hz.hnxiangtu.top/gtudjjcrmt.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.xuetiantiany.cn/gtihzoyapc.html

[Q88] 行转列（条件聚合）
来源：http://hz.xinyue.icu/gtiozppjxf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zhoulong.xyz/gtxqvpnbbf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.andypj.xyz/gtdcpvhfkk.html

[Q89] 判断表是否存在
来源：http://hz.c1oappe.top/gtygidbkmj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.andypj.xyz/gtlbeseqnh.html

[Q90] 生成序号列
来源：http://hz.jinghuilouyu.cn/gtdiqvkxfw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yuxming.cn/gthzcsrhcl.html

================================================================================
来源：http://hz.havefunace.top/gtzluuttdy.html

R. Bash 专题
来源：http://hz.yongpay.top/gtkuuubcmu.html

================================================================================
来源：http://hz.hongshengwenyu.top/gttvaesemt.html

[R01] shebang 与严格模式
来源：http://hz.jiagoushi.top/gtquikjlen.html

#!/usr/bin/env bash
来源：http://hz.gzhubu.top/gtydjvqyks.html

set -euo pipefail
来源：http://hz.0kj1m.cn/gtwcvuipif.html

[R02] 变量赋值与使用
来源：http://hz.jiagoushi.top/gtunbymkxy.html

name="Tom"; echo "$name"
来源：http://hz.hnxiangtu.top/gttllybndb.html

[R03] 只读变量
来源：http://hz.dianchejie.cn/gtozjzrweh.html

readonly PI=3.14
来源：http://hz.zhongyouzk.top/gteplnmveu.html

[R04] 位置参数
来源：http://hz.andypj.xyz/gtbfycmrti.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.jinqigfzy.top/gtnpvtywqn.html

[R05] 参数默认值
来源：http://hz.zdqjudy.top/gtxcexsrjv.html

name="${1:-default}"
来源：http://hz.xuanzx.com/gtuckckjzw.html

[R06] 判断命令是否存在
来源：http://hz.daxiang520.top/gtvjznufgx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.guannengcc.top/gtertcdbsl.html

[R07] if 判断文件
来源：http://hz.tianlin.xyz/gttjsskpsh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.316326.xyz/gtsgoduubb.html

[R08] 数值比较
来源：http://hz.xylfe.cn/gtoafkeiwd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.52xcode.cn/gteitvxnjf.html

[R09] 字符串比较
来源：http://hz.ivvv.top/gtapqjujuk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.xylfe.cn/gthlolhxus.html

[R10] 正则匹配
来源：http://hz.shuidangran.top/gtwyelmwti.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.tian-w.cn/gtebsxjapc.html

[R11] case 多分支
来源：http://hz.cashguo.top/gtorehjjzf.html

case "$1" in
来源：http://hz.chenjidiqi.icu/gtgxwwkffy.html

start) echo "启动" ;;
来源：http://hz.yj20258888.top/gtryyynknm.html

stop)  echo "停止" ;;
来源：http://hz.cqqwz.cn/gtgpxldopt.html

*)     echo "未知命令" ;;
来源：http://hz.mhx1999.top/gtrfmmasgt.html

esac
来源：http://hz.xingfuxueyuan.xyz/gtknehzwit.html

[R12] for 遍历文件
来源：http://hz.hammf.cn/gtpnulcihu.html

for f in *.txt; do echo "$f"; done
来源：http://hz.xylfe.cn/gtzafsssgx.html

[R13] for 计数循环
来源：http://hz.316326.xyz/gtkyzxnosd.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.birdmap.top/gtntrsghuk.html

[R14] C 风格 for
来源：http://hz.ydjk.org.cn/gtmpowhynz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.xziqi.cn/gtucyhizsc.html

[R15] while 逐行读文件
来源：http://hz.xylfe.cn/gtsiggmzgt.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.zhijiandao.cn/gtfddqbxeg.html

[R16] until 等待条件
来源：http://hz.hfpthk.cn/gtypjmiqja.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jqgufenzy.top/gthvrutypi.html

[R17] 数组定义与取值
来源：http://hz.fengsongda.top/gteppmhepp.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.shuidangran.top/gtteavpirt.html

[R18] 遍历数组
来源：http://hz.yuanzhike.top/gtxzgxdtka.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.yvedp.cn/gtmiokbawg.html

[R19] 数组长度
来源：http://hz.yj20258.top/gtkxdsdsjt.html

echo "${#arr[@]}"
来源：http://hz.xuanzx.com/gtzcuherrh.html

[R20] 关联数组（字典）
来源：http://hz.yongpay.top/gtzisabchj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.jqgfzy.top/gtxxlleidb.html

[R21] 字符串长度
来源：http://hz.zhixingplan.top/gtnjodnufl.html

echo "${#s}"
来源：http://hz.jqgufenzy.top/gtqwdheqts.html

[R22] 截取子串
来源：http://hz.ivvv.top/gtbrunkutg.html

echo "${s:0:5}"
来源：http://hz.nanxuanxn.top/gttrkueckh.html

[R23] 字符串替换
来源：http://hz.jlsjyb.cn/gthifsgdjm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.nanxinkj.top/gtknddpehw.html

[R24] 大小写转换
来源：http://hz.zhixingplan.top/gtwrjziauj.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.ydjk.org.cn/gtxenmhnkd.html

[R25] 去后缀 / 去前缀
来源：http://hz.jianghu66.top/gtoupdrjad.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.vqdsnc.cn/gtivnfuolv.html

[R26] 命令替换
来源：http://hz.xingfuxueyuan.xyz/gtbsruxwly.html

now=$(date +%F); echo "$now"
来源：http://hz.haohaochexian.top/gtbftewzcz.html

[R27] 算术展开
来源：http://hz.ppjwa.cn/gtsyppfymy.html

echo $((1 + 2 * 3))
来源：http://hz.dianchejie.cn/gtwnbthgaq.html

[R28] 浮点运算
来源：http://hz.hywenlv.cn/gtmkqwpcxh.html

echo "scale=2; 10/3" | bc
来源：http://hz.52xcode.cn/gtjmxtfcsk.html

[R29] 定义函数
来源：http://hz.316326.xyz/gtgzypgyiw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jianghu66.top/gtdlbvmkni.html

[R30] 函数返回状态码
来源：http://hz.guannengcc.top/gtwchmgiuz.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.sweek.top/gtsarlshrq.html

[R31] 局部变量
来源：http://hz.quarkkingdee.top/gtisyxpnfq.html

f() { local x=1; echo "$x"; }
来源：http://hz.sysykeji.top/gtbetqyoyb.html

[R32] 参数个数校验
来源：http://hz.hfpthk.cn/gtoqvnntpq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.zhongyouzk.top/gtauiumpqp.html

[R33] 捕获错误并提示行号
来源：http://hz.cheryme.top/gtmlnaipjc.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jinghuilouyu.cn/gtpypmurke.html

[R34] 退出时清理
来源：http://hz.daria6918.cn/gtpciveokx.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.ehwqpu.com/gtzfnzdebo.html

[R35] 后台执行并等待
来源：http://hz.yonumen.top/gtcvdcekdp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.0kj1m.cn/gtcglucivs.html

[R36] 并发执行多个任务
来源：http://hz.andypj.xyz/gtyfaxfpgp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.hongshengwenyu.top/gtztxirvwc.html

[R37] 把输出赋给变量
来源：http://hz.havefunace.top/gtkbptcvqt.html

files=$(ls -1)
来源：http://hz.zdqjudy.top/gtonciuoby.html

[R38] 管道串联
来源：http://hz.pycfn.com/gtcnexhiqb.html

cat a.txt | grep -i error | wc -l
来源：http://hz.redwolf501.top/gtrxmaulwd.html

[R39] 重定向标准输出与错误
来源：http://hz.chenzaomai.com/gtnifaxxha.html

cmd > out.log 2>&1
来源：http://hz.52xcode.cn/gtpobyhfuq.html

[R40] 追加写日志
来源：http://hz.shangyingyoupin.top/gtqjbabkgo.html

echo "log" >> out.log
来源：http://hz.redwolf501.top/gtyxvfnokt.html

[R41] 丢弃输出
来源：http://hz.cucudq.cn/gtdrbswvhj.html

cmd >/dev/null 2>&1
来源：http://hz.hongshengwenyu.top/gtkajsmvht.html

[R42] 输入重定向
来源：http://hz.shuidangran.top/gtxsykqnvn.html

wc -l < a.txt
来源：http://hz.9152youxi.cn/gtstvnczwd.html

[R43] 按名字查找文件
来源：http://hz.hammf.cn/gtkajqcybj.html

find . -name "*.log" -type f
来源：http://hz.fzhhl.top/gtzggiplce.html

[R44] 按修改时间查找
来源：http://hz.hysaishi.cn/gtqcndnhfn.html

find . -mtime -7 -type f
来源：http://hz.yvedp.cn/gtihdejykl.html

[R45] 批量删除
来源：http://hz.yj20258888.top/gtrapcdylf.html

find . -name "*.tmp" -delete
来源：http://hz.shanyushiyangkeji.top/gtuziutffv.html

[R46] 递归替换文件内容
来源：http://hz.guannengcc.top/gtlvtoblue.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.ybcxt.top/gtzotvpung.html

[R47] sed 单行替换
来源：http://hz.yj20258.top/gthnppmajm.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.aibaodan.cn/gtypzvcpji.html

[R48] awk 取指定列
来源：http://hz.cucudq.cn/gtdmvkpqro.html

awk '{print $1, $3}' a.txt
来源：http://hz.hnxiangtu.top/gtgsgohdus.html

[R49] awk 带条件
来源：http://hz.ivvv.top/gtpdtjkgoi.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yj20258.top/gtaidivpzg.html

[R50] awk 求和
来源：http://hz.gaohongyu789.top/gtlvwvixkl.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yvedp.cn/gtxkmpxbao.html

[R51] 排序去重取前几
来源：http://hz.wangshuangyany.cn/gtsgipwqbq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.quarkkingdee.top/gtufuqdmfb.html

[R52] 统计行数
来源：http://hz.hongshengwenyu.top/gtpdwsbgzt.html

wc -l a.txt
来源：http://hz.shanyushiyangtech.top/gtwtdzhdwz.html

[R53] 查看文件头与实时尾
来源：http://hz.haohaochexian.top/gtviklqspw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.svipenyu.cn/gtgyaqftbw.html

[R54] 比较两个文件
来源：http://hz.gotoacloud.top/gttzrztkac.html

diff a.txt b.txt
来源：http://hz.chenlongwang.top/gtvzcygdiu.html

[R55] 压缩与解压
来源：http://hz.316326.xyz/gtjldyzkzf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.havefunace.top/gtncgxrbda.html

[R56] 远程拷贝
来源：http://hz.yj20258.top/gtrfdghiyg.html

scp file user@host:/path/
来源：http://hz.ybcxt.top/gtcwjfmlau.html

[R57] 远程执行命令
来源：http://hz.chenzaomai.com/gtvaupukxs.html

ssh user@host 'uptime'
来源：http://hz.yueranfly.top/gtthnftvfh.html

[R58] 下载文件
来源：http://hz.shanyushiyangkeji.top/gtorbkqyrx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.zdqjudy.top/gtpnsoubiw.html

[R59] 发 POST JSON
来源：http://hz.kuanghao11.cn/gturrmhvql.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.wangdashe.top/gtkyftoaab.html

[R60] 只看 HTTP 状态码
来源：http://hz.xylfe.cn/gtutueoolu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jlsjyb.cn/gtzdlaozsl.html

[R61] 磁盘占用
来源：http://hz.nanxinkj.top/gtipvjmfnd.html

df -h;  du -sh *
来源：http://hz.xziqi.cn/gtwhvceiiv.html

[R62] 找最占空间的文件
来源：http://hz.gogol.net.cn/gtaqruofob.html

du -ah . | sort -rh | head -10
来源：http://hz.yongpay.top/gthpfpgbby.html

[R63] 内存与进程
来源：http://hz.ydzc1.top/gtgwveagvs.html

free -h;  ps aux | grep nginx
来源：http://hz.hfpthk.cn/gtgwrurzra.html

[R64] 结束进程
来源：http://hz.xziqi.cn/gtnonuhcgt.html

kill -9 $(pgrep -f app.py)
来源：http://hz.chenzaomai.com/gtfbyaepvl.html

[R65] 查看端口占用
来源：http://hz.iojbl.cn/gtqehimrce.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.fengsongda.top/gttbkoprzd.html

[R66] 定时任务
来源：http://hz.aibaodan.cn/gtzivpgozq.html

crontab -e;  crontab -l
来源：http://hz.xziqi.cn/gtqyvlgtty.html

[R67] 生成随机十六进制串
来源：http://hz.smart0.xyz/gtumlffbbb.html

openssl rand -hex 16
来源：http://hz.zhoulong.xyz/gtgmvglqqi.html

[R68] 计算文件校验值
来源：http://hz.daria6918.cn/gtpcnhprvs.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yanxiufei.cn/gtgdscosyn.html

[R69] 生成随机密码
来源：http://hz.guannengcc.top/gtnuuwnhlm.html

head -c 16 /dev/urandom | base64
来源：http://hz.zhengqikj.top/gtuhxvglvq.html

[R70] 时间戳与互转
来源：http://hz.nanxuanxn.top/gtktychgbb.html

date +%s;  date -d @1700000000
来源：http://hz.jianghu66.top/gtcdqanzxs.html

[R71] 日期格式化
来源：http://hz.redwolf501.top/gtvpihqtij.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.guowangkeji.top/gtxeldkiqj.html

[R72] 等待端口就绪
来源：http://hz.zhoulong.xyz/gtsziiqiof.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.shangyingyoupin.top/gtouludydi.html

[R73] 分割大日志
来源：http://hz.cqqwz.cn/gtlqunvlqt.html

split -l 1000 big.log part_
来源：http://hz.ybcxt.top/gtrgzpiqet.html

[R74] 批量重命名
来源：http://hz.sweek.top/gtngewmuhj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.gzhubu.top/gtuvllogly.html

[R75] 导出环境变量
来源：http://hz.feifeiyinyue.top/gtyurvfqjr.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yanxiufei.cn/gtfzyjzqqj.html

[R76] 使用临时文件
来源：http://hz.gogol.net.cn/gtvnpwimxi.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.zdqjudy.top/gtsjdzxiko.html

[R77] 读取用户输入
来源：http://hz.haohaochexian.top/gtlpaeqjdd.html

read -rp "请输入: " ans
来源：http://hz.havefunace.top/gtsfbnxokl.html

[R78] 交互式菜单
来源：http://hz.zhoulong.xyz/gtgpzjxcuw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.ydzc1.top/gtepovpbzo.html

[R79] 解析命令行选项
来源：http://hz.xinyue.icu/gtilvzbijz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.tianlin.xyz/gteapsaxhs.html

[R80] 查看脚本执行耗时
来源：http://hz.sufxvd.cn/gtbtcdqdik.html

time ./run.sh
来源：http://hz.xuanzx.com/gtgtsjinfg.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtgwcmyfdl.html

S. C / C++ 专题
来源：http://hz.tian-w.cn/gtqntdyksh.html

================================================================================
来源：http://hz.cheryme.top/gtvuznqtmm.html

[S01] C：Hello World
来源：http://hz.cheryme.top/gtufknolbk.html

#include <stdio.h>
来源：http://hz.andypj.xyz/gtxkhtclxb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yj20258888.top/gtbzchvjts.html

[S02] C：变量与格式化输出
来源：http://hz.jianghu66.top/gtoqqufmue.html

int a = 10; printf("%d\n", a);
来源：http://hz.dashuyun.cn/gtuafxsvbq.html

[S03] C：读入整数
来源：http://hz.wangshuangyany.cn/gtchgrzcue.html

int x; scanf("%d", &x);
来源：http://hz.jinqigufen.top/gtzelcsrna.html

[S04] C：字符串复制
来源：http://hz.ehwqpu.com/gtfrlxydpp.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.gzhubu.top/gtjvtlcufw.html

[S05] C：字符串长度
来源：http://hz.jinqigufen.top/gtdrkzhghs.html

strlen(s)
来源：http://hz.zhiwuduotai.top/gtlxfshyuh.html

[S06] C：字符串比较
来源：http://hz.yj202588.top/gtogsavhti.html

strcmp(a, b) == 0
来源：http://hz.bjfxy.top/gtrcskkfpu.html

[S07] C：数组遍历求和
来源：http://hz.9152youxi.cn/gtcdrlyypj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.hywenlv.cn/gtxsozvosd.html

[S08] C：动态内存分配与释放
来源：http://hz.aizwys.cn/gttflvswmr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.mhx1999.top/gtexchykap.html

[S09] C：结构体定义与初始化
来源：http://hz.316326.xyz/gtwwdmflrc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.chenlongwang.top/gtqgklgjkq.html

[S10] C：指针与解引用
来源：http://hz.zhongyouzk.top/gtuonhsbeq.html

int *p = &a;  *p = 5;
来源：http://hz.xuanzx.com/gtqrurwswq.html

[S11] C：逐行读文件
来源：http://hz.zhijiandao.cn/gtazksbojd.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.shuidangran.top/gtrgklhnvl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yonumen.top/gtkzwswzvr.html

fclose(f);
来源：http://hz.c1oappe.top/gtvhvnlbwt.html

[S12] C：写文件
来源：http://hz.cqqwz.cn/gtypzfotnc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.cheryme.top/gtvekvclpx.html

[S13] C：宏定义
来源：http://hz.guowangkeji.top/gtwldrsqpm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.jyoumei.cn/gtpldzabxb.html

[S14] C：枚举
来源：http://hz.zycfv.cn/gtnimwgifx.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.feifeiyinyue.top/gtfvfnylfp.html

[S15] C：类型转换
来源：http://hz.meibo888.top/gtdidxdjeu.html

(double) a / b
来源：http://hz.ehwqpu.com/gtdakgrzpj.html

[S16] C：位操作置位
来源：http://hz.jianghu66.top/gtspnnxxcc.html

x |= (1 << 3);
来源：http://hz.yuxming.cn/gtwbvjqhax.html

[S17] C：安全拼接字符串
来源：http://hz.shzxlz.cn/gtxqltlecs.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.andypj.xyz/gtexakcbxo.html

[S18] C：命令行参数
来源：http://hz.yj202588.top/gthkcpxxks.html

int main(int argc, char **argv)
来源：http://hz.meibo888.top/gthtsmhrsz.html

[S19] C：快速排序
来源：http://hz.hywenlv.cn/gtnksvwwko.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.shanyushiyangtech.top/gtkjqpsxnr.html

[S20] C：二分查找
来源：http://hz.yj202588.top/gtlhqkilhu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.ppjwa.cn/gtxgpabeua.html

[S21] C：字符类别判断
来源：http://hz.meibo888.top/gtkqxromig.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.tianlin.xyz/gtgbzmhxcb.html

[S22] C：字符串转数字
来源：http://hz.pengpengdd.cyou/gtqouwqhaj.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.nanxinkj.top/gtlylymods.html

[S23] C：随机数
来源：http://hz.zdqjudy.top/gtkiwmnqrc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.sysykeji.top/gtnyfodmzs.html

[S24] C：获取本地时间
来源：http://hz.ivvv.top/gtvfyrlelb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.jinqigufen.top/gthtmsucuh.html

[S25] C：内存拷贝
来源：http://hz.hywenlv.cn/gtfsxtpeim.html

memcpy(dst, src, n);
来源：http://hz.gogol.net.cn/gtvwdycebq.html

[S26] C：内存清零
来源：http://hz.xylfe.cn/gtvavurrkh.html

memset(a, 0, sizeof a);
来源：http://hz.tianlin.xyz/gtsbufysvy.html

[S27] C：定义常量
来源：http://hz.ywan-chungtsiang.top/gtmkxzoqjl.html

const double PI = 3.14159;
来源：http://hz.zhijiandao.cn/gtmuyddkgm.html

[S28] C：静态变量
来源：http://hz.jinghuilouyu.cn/gthzwhqpux.html

static int counter = 0;
来源：http://hz.vqdsnc.cn/gtisyvgzpj.html

[S29] C：变参函数
来源：http://hz.ybcxt.top/gtzpwjtlvu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jlsjyb.cn/gtcokahhls.html

[S30] C：头文件保护
来源：http://hz.aibaodan.cn/gtbgzpbmvt.html

#ifndef X_H
来源：http://hz.hfpthk.cn/gtvvuuhjml.html

#define X_H
来源：http://hz.wangdashe.top/gtisgtzzta.html

#endif
来源：http://hz.ppjwa.cn/gtmvhdwvkk.html

[S31] C++：Hello World
来源：http://hz.smart0.xyz/gtpmdmniif.html

#include <iostream>
来源：http://hz.meibo888.top/gtfdgskwzs.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.xylfe.cn/gtuqknsune.html

[S32] C++：字符串
来源：http://hz.hongshengwenyu.top/gtpsytafix.html

std::string s = "hi";  s += "!";
来源：http://hz.snrcjt.cn/gtcckodfdt.html

[S33] C++：vector 增删
来源：http://hz.svipenyu.cn/gtsjtxlesf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.kuanghao11.cn/gtjafizsnj.html

[S34] C++：遍历 vector
来源：http://hz.cdnleiting.top/gtfqncdmvd.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.feifeiyinyue.top/gttcukluyw.html

[S35] C++：map
来源：http://hz.daria6918.cn/gtiftgndpu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.guowangkeji.top/gtivoateym.html

[S36] C++：unordered_map
来源：http://hz.hnqzz.top/gtydgcqlrn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.chenlongwang.top/gtimvsbslj.html

[S37] C++：set
来源：http://hz.yuanzhike.top/gtedmedpjh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.ywan-chungtsiang.top/gtqpxyuzlv.html

[S38] C++：排序
来源：http://hz.iojbl.cn/gtmmjgiita.html

std::sort(v.begin(), v.end());
来源：http://hz.jqgufenzy.top/gtfpsenhnx.html

[S39] C++：自定义比较器排序
来源：http://hz.yj202588.top/gtsowqrqvl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.ppjwa.cn/gtgpjnivrn.html

[S40] C++：查找元素
来源：http://hz.jiagoushi.top/gtwbgvebsr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.zycfv.cn/gtkmamznmw.html

[S41] C++：类与构造函数
来源：http://hz.jianghu66.top/gtoyiectus.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.zhixingplan.top/gtrzdwlupo.html

[S42] C++：继承与虚函数
来源：http://hz.c1oappe.top/gtalmixagh.html

class B : public Base { public: void f() override {} };
来源：http://hz.yvedp.cn/gtjypcqgov.html

[S43] C++：智能指针
来源：http://hz.yongpay.top/gtrvlgtioq.html

auto p = std::make_unique<int>(5);
来源：http://hz.wangshuangyany.cn/gtamlnzdcl.html

[S44] C++：引用传参
来源：http://hz.xuanzx.com/gttrfhpaxv.html

void inc(int &x) { ++x; }
来源：http://hz.fengsongda.top/gtjpgmixxr.html

[S45] C++：lambda
来源：http://hz.zdqjudy.top/gtzxwybhfz.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.nwbrower.top/gtyibormbw.html

[S46] C++：函数模板
来源：http://hz.c1oappe.top/gttgduqoxa.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yuanzhike.top/gtpfbcdroa.html


<!-- 参考信息 -->