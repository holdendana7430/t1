代发 wailian999

ROLLBACK TO sp1;
来源：http://hz.wangdashe.top/gtbzujmqbu.html

[Q69] 查看执行计划
来源：http://hz.jianghu66.top/gtuglalvyo.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.havefunace.top/gtisctcmks.html

[Q70] 更新统计信息
来源：http://hz.jqgufenzy.top/gttbfvoqef.html

ANALYZE TABLE users;
来源：http://hz.ywan-chungtsiang.top/gtdjdievni.html

[Q71] 查看建表语句
来源：http://hz.zhoulong.xyz/gtzzcrwqzo.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.tanke756.top/gtssaarfni.html

[Q72] 查看索引
来源：http://hz.chenzaomai.com/gtfqmlltca.html

SHOW INDEX FROM users;
来源：http://hz.hammf.cn/gtviuutqvn.html

[Q73] 查看表状态
来源：http://hz.andypj.xyz/gtrqjrtcen.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.ydzc1.top/gtonzdxljk.html

[Q74] 强制使用索引
来源：http://hz.dashuyun.cn/gtiookwxlr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.316326.xyz/gtqyujxbjv.html

[Q75] 日期格式化
来源：http://hz.ydjk.org.cn/gtyixarzhl.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.cdnleiting.top/gtiwvhwlnd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.iojbl.cn/gtrddupbti.html

[Q76] 按天统计
来源：http://hz.guowangkeji.top/gtlhpghxjo.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jinyuanbaomall.cn/gtezmehubm.html

[Q77] 时间加减
来源：http://hz.yangfankeji.com/gthuljdcoq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.cqqwz.cn/gtrtmczyqw.html

[Q78] 当前时间
来源：http://hz.fengsongda.top/gtasdgldkw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.gzhubu.top/gthcfqxnvo.html

[Q79] 字符串拼接
来源：http://hz.tian-w.cn/gtbsiymsbb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.zycfv.cn/gtjyvkgmzf.html

[Q80] 字符串截取
来源：http://hz.aibaodan.cn/gtgmyxstnx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.hammf.cn/gtzusehnwi.html

[Q81] 字符串替换
来源：http://hz.jyoumei.cn/gtnmvgxnby.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.gotoacloud.top/gtgdbgljzb.html

[Q82] 字符长度与字节长度
来源：http://hz.zhongyouzk.top/gtzmmjkqat.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yj20258.top/gtnrnahano.html

[Q83] 大小写转换
来源：http://hz.jlsjyb.cn/gtgriwhcle.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.tanke756.top/gthcddzcvx.html

[Q84] 去除首尾空格
来源：http://hz.yongpay.top/gtttbavynw.html

SELECT TRIM(name) FROM users;
来源：http://hz.yj20258888.top/gtmdceqvmz.html

[Q85] 数值取整
来源：http://hz.ivvv.top/gtepiiikdo.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.gogol.net.cn/gtvjaexpza.html

[Q86] 读取 JSON 字段
来源：http://hz.tanke756.top/gtquagqbhb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.snrcjt.cn/gtvoybeajk.html

[Q87] JSON 字段做条件
来源：http://hz.52xcode.cn/gttiolncrk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.quarkkingdee.top/gtkxandiuj.html

[Q88] 行转列（条件聚合）
来源：http://hz.aibaodan.cn/gtwzqygiiz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.sxryk.cn/gtpqcyniio.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yvedp.cn/gtgliepsyg.html

[Q89] 判断表是否存在
来源：http://hz.daxiang520.top/gteoelkbeh.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.guannengcc.top/gtbsdhhqgl.html

[Q90] 生成序号列
来源：http://hz.haohaochexian.top/gtrayslefl.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.nwbrower.top/gtotosdrpd.html

================================================================================
来源：http://hz.tian-w.cn/gtemxsaljz.html

R. Bash 专题
来源：http://hz.redwolf501.top/gtvnacdzaf.html

================================================================================
来源：http://hz.yj20258.top/gtzwvpbqom.html

[R01] shebang 与严格模式
来源：http://hz.birdmap.top/gtuucqebsb.html

#!/usr/bin/env bash
来源：http://hz.xuetiantiany.cn/gttzdcvuol.html

set -euo pipefail
来源：http://hz.bjfxy.top/gtgxkwkhec.html

[R02] 变量赋值与使用
来源：http://hz.sufxvd.cn/gtiebxsucl.html

name="Tom"; echo "$name"
来源：http://hz.chenlongwang.top/gthappjlma.html

[R03] 只读变量
来源：http://hz.tianlin.xyz/gtbhzmdyvs.html

readonly PI=3.14
来源：http://hz.chenlongwang.top/gtnbnpzscr.html

[R04] 位置参数
来源：http://hz.jinghuilouyu.cn/gtgdlfeddl.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.ywan-chungtsiang.top/gtoiabjaxh.html

[R05] 参数默认值
来源：http://hz.jqgfzy.top/gtxccefctk.html

name="${1:-default}"
来源：http://hz.sxryk.cn/gtseimjkfu.html

[R06] 判断命令是否存在
来源：http://hz.pycfn.com/gtolnlgqzb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yueranfly.top/gtwbueqtah.html

[R07] if 判断文件
来源：http://hz.xylfe.cn/gtrgzazgqq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.pycfn.com/gturvtbrkz.html

[R08] 数值比较
来源：http://hz.mhx1999.top/gtrmawdskx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jqgfzy.top/gtrgvyjdnq.html

[R09] 字符串比较
来源：http://hz.xingfuxueyuan.xyz/gtabfjhqct.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.aizwys.cn/gtjngcdfpc.html

[R10] 正则匹配
来源：http://hz.nanxuanxn.top/gtuaeoflqx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.ybcxt.top/gtgakppfzj.html

[R11] case 多分支
来源：http://hz.pengpengdd.cyou/gtapxsschn.html

case "$1" in
来源：http://hz.smart0.xyz/gtvfhnhayg.html

start) echo "启动" ;;
来源：http://hz.nanxinkj.top/gtdfoblxtf.html

stop)  echo "停止" ;;
来源：http://hz.yongpay.top/gtwknydges.html

*)     echo "未知命令" ;;
来源：http://hz.ybcxt.top/gtqofdcevi.html

esac
来源：http://hz.tianlin.xyz/gtpjqbmfzx.html

[R12] for 遍历文件
来源：http://hz.quarkkingdee.top/gtghsusdsz.html

for f in *.txt; do echo "$f"; done
来源：http://hz.daxiang520.top/gtssafaaeo.html

[R13] for 计数循环
来源：http://hz.daria6918.cn/gtqdkhbynu.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yj20258888.top/gtcduykwcq.html

[R14] C 风格 for
来源：http://hz.pengpengdd.cyou/gtdlkklezs.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.zhongyouzk.top/gtrlytbzil.html

[R15] while 逐行读文件
来源：http://hz.meibo888.top/gtgvacrbmw.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.tanke756.top/gtyfzdjbgo.html

[R16] until 等待条件
来源：http://hz.jianghu66.top/gtggetyicx.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.nanxinkj.top/gtulqphnyh.html

[R17] 数组定义与取值
来源：http://hz.zdqjudy.top/gtznleycnw.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yangfankeji.com/gtvipspufy.html

[R18] 遍历数组
来源：http://hz.xziqi.cn/gtbojdwjni.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.tanke756.top/gtgzcvvkyu.html

[R19] 数组长度
来源：http://hz.hysaishi.cn/gtglfjxoes.html

echo "${#arr[@]}"
来源：http://hz.jiagoushi.top/gtucparsjh.html

[R20] 关联数组（字典）
来源：http://hz.yanxiufei.cn/gtmzaftehg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.bjfxy.top/gtmbqqyfii.html

[R21] 字符串长度
来源：http://hz.yangfankeji.com/gtoznuflti.html

echo "${#s}"
来源：http://hz.svipenyu.cn/gtubxjeshm.html

[R22] 截取子串
来源：http://hz.andypj.xyz/gtjdjcrrrk.html

echo "${s:0:5}"
来源：http://hz.hammf.cn/gtajwflyhu.html

[R23] 字符串替换
来源：http://hz.c1oappe.top/gtbpaqyayl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jqgfzy.top/gtegnsqzdk.html

[R24] 大小写转换
来源：http://hz.birdmap.top/gtftylbumh.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.fengsongda.top/gthkglbbck.html

[R25] 去后缀 / 去前缀
来源：http://hz.jinghuilouyu.cn/gtnitxkgnu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.hammf.cn/gtmsqfyqoz.html

[R26] 命令替换
来源：http://hz.jiagoushi.top/gtkqmgnokl.html

now=$(date +%F); echo "$now"
来源：http://hz.nwbrower.top/gtignnohzq.html

[R27] 算术展开
来源：http://hz.shangyingyoupin.top/gtxqexmnxh.html

echo $((1 + 2 * 3))
来源：http://hz.shangyingyoupin.top/gtfbyzxnwg.html

[R28] 浮点运算
来源：http://hz.fzhhl.top/gtauaiiuap.html

echo "scale=2; 10/3" | bc
来源：http://hz.yonumen.top/gtnuzannsw.html

[R29] 定义函数
来源：http://hz.hysaishi.cn/gtovgfygnc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.shangyingyoupin.top/gtwcgbwned.html

[R30] 函数返回状态码
来源：http://hz.jyoumei.cn/gtqrbyojvf.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.feifeiyinyue.top/gtsymupfji.html

[R31] 局部变量
来源：http://hz.sufxvd.cn/gtwzbiudri.html

f() { local x=1; echo "$x"; }
来源：http://hz.zhengqikj.top/gtxglccdzr.html

[R32] 参数个数校验
来源：http://hz.yvedp.cn/gtwfaebikn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jqgfzy.top/gtremjmvmx.html

[R33] 捕获错误并提示行号
来源：http://hz.jyoumei.cn/gtlpjlltug.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zhengqikj.top/gtpnyesqfb.html

[R34] 退出时清理
来源：http://hz.guowangkeji.top/gtxaxxnpnf.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.gotoacloud.top/gtprvgxzfi.html

[R35] 后台执行并等待
来源：http://hz.xinyue.icu/gttgixnvkg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yangfankeji.com/gtqrxhcylm.html

[R36] 并发执行多个任务
来源：http://hz.zdqjudy.top/gtjpviaxml.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.sweek.top/gtukmbcefc.html

[R37] 把输出赋给变量
来源：http://hz.gaohongyu789.top/gtxivczovw.html

files=$(ls -1)
来源：http://hz.shzxlz.cn/gtqfnjcpsn.html

[R38] 管道串联
来源：http://hz.52xcode.cn/gtvlciyspe.html

cat a.txt | grep -i error | wc -l
来源：http://hz.zhengqikj.top/gtlvkqhmcq.html

[R39] 重定向标准输出与错误
来源：http://hz.cqqwz.cn/gtbzktkyzj.html

cmd > out.log 2>&1
来源：http://hz.yj202588.top/gtnplrcqoo.html

[R40] 追加写日志
来源：http://hz.9152youxi.cn/gtobknrhio.html

echo "log" >> out.log
来源：http://hz.tian-w.cn/gticngckia.html

[R41] 丢弃输出
来源：http://hz.havefunace.top/gtjnfvogrx.html

cmd >/dev/null 2>&1
来源：http://hz.birdmap.top/gtlcpjvfvd.html

[R42] 输入重定向
来源：http://hz.iojbl.cn/gtohabojoq.html

wc -l < a.txt
来源：http://hz.iojbl.cn/gtdujufrlj.html

[R43] 按名字查找文件
来源：http://hz.ehwqpu.com/gtzfmfmcyl.html

find . -name "*.log" -type f
来源：http://hz.zhaomingkeji.xyz/gtqvwjmbtp.html

[R44] 按修改时间查找
来源：http://hz.hongshengwenyu.top/gtkwmfjehz.html

find . -mtime -7 -type f
来源：http://hz.gogol.net.cn/gtncgkyjcz.html

[R45] 批量删除
来源：http://hz.zhaomingkeji.xyz/gtbaqmmpiu.html

find . -name "*.tmp" -delete
来源：http://hz.jianghu66.top/gtjalkhiko.html

[R46] 递归替换文件内容
来源：http://hz.zhaomingkeji.xyz/gtfpqedein.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yj20258888.top/gthakxvpeg.html

[R47] sed 单行替换
来源：http://hz.gogol.net.cn/gtrdpdqgze.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.xuetiantiany.cn/gtikwsoxts.html

[R48] awk 取指定列
来源：http://hz.yuxming.cn/gtvowhbihs.html

awk '{print $1, $3}' a.txt
来源：http://hz.zhoulong.xyz/gtyemwrozb.html

[R49] awk 带条件
来源：http://hz.316326.xyz/gtkfzvqtfz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.wangshuangyany.cn/gtylmqukry.html

[R50] awk 求和
来源：http://hz.zycfv.cn/gtyeahtluo.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.daxiang520.top/gtvxwnoxbh.html

[R51] 排序去重取前几
来源：http://hz.hongshengwenyu.top/gtfxrdzgiv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.gogol.net.cn/gtbsibxfsw.html

[R52] 统计行数
来源：http://hz.316326.xyz/gtflnwykxx.html

wc -l a.txt
来源：http://hz.jinqigfzy.top/gtwqwzwrod.html

[R53] 查看文件头与实时尾
来源：http://hz.jinghuilouyu.cn/gtnyczareb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.pengpengdd.cyou/gttwxknksv.html

[R54] 比较两个文件
来源：http://hz.jinqigfzy.top/gtjtlhiukq.html

diff a.txt b.txt
来源：http://hz.9152youxi.cn/gtmdlbceen.html

[R55] 压缩与解压
来源：http://hz.jyoumei.cn/gtiavctlru.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.ehwqpu.com/gttkjauaxd.html

[R56] 远程拷贝
来源：http://hz.yangfankeji.com/gtbskmmwvy.html

scp file user@host:/path/
来源：http://hz.jqgfzy.top/gtzxbadpgr.html

[R57] 远程执行命令
来源：http://hz.c1oappe.top/gtesulfnad.html

ssh user@host 'uptime'
来源：http://hz.gaohongyu789.top/gttmavrpzu.html

[R58] 下载文件
来源：http://hz.shuidangran.top/gtcugsrqiz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.daria6918.cn/gtheruspbi.html

[R59] 发 POST JSON
来源：http://hz.aizwys.cn/gtubhsafsb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.52xcode.cn/gthpexmjho.html

[R60] 只看 HTTP 状态码
来源：http://hz.xingfuxueyuan.xyz/gtmrwwvwmj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.xziqi.cn/gtgzbvfyvo.html

[R61] 磁盘占用
来源：http://hz.havefunace.top/gtitsapysd.html

df -h;  du -sh *
来源：http://hz.jiagoushi.top/gtflojhagz.html

[R62] 找最占空间的文件
来源：http://hz.yj20258888.top/gtunzallte.html

du -ah . | sort -rh | head -10
来源：http://hz.nwbrower.top/gtmptujvfh.html

[R63] 内存与进程
来源：http://hz.xziqi.cn/gtenciyplc.html

free -h;  ps aux | grep nginx
来源：http://hz.ydzc1.top/gtekwxlrhh.html

[R64] 结束进程
来源：http://hz.ydjk.org.cn/gtlpjyuypi.html

kill -9 $(pgrep -f app.py)
来源：http://hz.vqdsnc.cn/gtgjjotsoj.html

[R65] 查看端口占用
来源：http://hz.sufxvd.cn/gtpzarcrqr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.mhx1999.top/gtcvzvtyxt.html

[R66] 定时任务
来源：http://hz.xziqi.cn/gteoopyfzs.html

crontab -e;  crontab -l
来源：http://hz.havefunace.top/gtyjdawtck.html

[R67] 生成随机十六进制串
来源：http://hz.hongshengwenyu.top/gtaszqdwat.html

openssl rand -hex 16
来源：http://hz.smart0.xyz/gtuikoscmx.html

[R68] 计算文件校验值
来源：http://hz.xuetiantiany.cn/gtetckiinm.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.dianchejie.cn/gtjvkxmvka.html

[R69] 生成随机密码
来源：http://hz.shzxlz.cn/gtgkazelzk.html

head -c 16 /dev/urandom | base64
来源：http://hz.nanxinkj.top/gtnchwlumt.html

[R70] 时间戳与互转
来源：http://hz.jqgfzy.top/gtdytpvtks.html

date +%s;  date -d @1700000000
来源：http://hz.zdqjudy.top/gtclgztpub.html

[R71] 日期格式化
来源：http://hz.zdqjudy.top/gthancwslz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.ydzc1.top/gtejkydgij.html

[R72] 等待端口就绪
来源：http://hz.vqdsnc.cn/gtnfluvfar.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.birdmap.top/gtlmtlussk.html

[R73] 分割大日志
来源：http://hz.316326.xyz/gtqqkwcrdq.html

split -l 1000 big.log part_
来源：http://hz.yuanzhike.top/gttirjhnxh.html

[R74] 批量重命名
来源：http://hz.c1oappe.top/gtxbufonwi.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.yangfankeji.com/gtqitnckng.html

[R75] 导出环境变量
来源：http://hz.guannengcc.top/gtesfdltif.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.tianlin.xyz/gtxavjyhmu.html

[R76] 使用临时文件
来源：http://hz.zhaomingkeji.xyz/gtyzelxuyj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.dianchejie.cn/gtjllkscyh.html

[R77] 读取用户输入
来源：http://hz.yuanzhike.top/gtiodnfcnt.html

read -rp "请输入: " ans
来源：http://hz.daxiang520.top/gtqmiplron.html

[R78] 交互式菜单
来源：http://hz.zhongyouzk.top/gtarwnnpgb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yueranfly.top/gtolhpuefa.html

[R79] 解析命令行选项
来源：http://hz.hysaishi.cn/gtadjqkqmm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.smart0.xyz/gtojnvywnr.html

[R80] 查看脚本执行耗时
来源：http://hz.316326.xyz/gtiqetcevt.html

time ./run.sh
来源：http://hz.daria6918.cn/gtedmvvqsf.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtcxzafpvo.html

S. C / C++ 专题
来源：http://hz.havefunace.top/gtvliywjlb.html

================================================================================
来源：http://hz.yangfankeji.com/gtnvbgmvss.html

[S01] C：Hello World
来源：http://hz.xziqi.cn/gtkabdlqex.html

#include <stdio.h>
来源：http://hz.smart0.xyz/gtbfsxfryi.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.sufxvd.cn/gtjqfpjqfi.html

[S02] C：变量与格式化输出
来源：http://hz.chenjidiqi.icu/gtixbshnoc.html

int a = 10; printf("%d\n", a);
来源：http://hz.sufxvd.cn/gtfnkfvvyw.html

[S03] C：读入整数
来源：http://hz.hammf.cn/gtmunkchyl.html

int x; scanf("%d", &x);
来源：http://hz.havefunace.top/gtednmhnbz.html

[S04] C：字符串复制
来源：http://hz.hongshengwenyu.top/gtpkyxkizo.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.sweek.top/gthynwalog.html

[S05] C：字符串长度
来源：http://hz.vqdsnc.cn/gtrsrpwgei.html

strlen(s)
来源：http://hz.hongshengwenyu.top/gtpfnxvemr.html

[S06] C：字符串比较
来源：http://hz.hammf.cn/gtlbiikdkg.html

strcmp(a, b) == 0
来源：http://hz.haohaochexian.top/gtctetwtzi.html

[S07] C：数组遍历求和
来源：http://hz.zhiwuduotai.top/gtalxfcqep.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.aibaodan.cn/gtofqqpoza.html

[S08] C：动态内存分配与释放
来源：http://hz.sufxvd.cn/gtrwhxdtdz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.chenlongwang.top/gthxedjgzc.html

[S09] C：结构体定义与初始化
来源：http://hz.nanxinkj.top/gtgjttxyhh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.ywan-chungtsiang.top/gtmbnhehyf.html

[S10] C：指针与解引用
来源：http://hz.zhijiandao.cn/gttdvrdvca.html

int *p = &a;  *p = 5;
来源：http://hz.meibo888.top/gtbguaiytx.html

[S11] C：逐行读文件
来源：http://hz.c1oappe.top/gtnjzepihl.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.sxryk.cn/gtdhywrazj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.xingfuxueyuan.xyz/gtpnefyrej.html

fclose(f);
来源：http://hz.daria6918.cn/gtnmcfunrb.html

[S12] C：写文件
来源：http://hz.yj202588.top/gtqqurxdmw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.gzhubu.top/gtpwcbitzy.html

[S13] C：宏定义
来源：http://hz.redwolf501.top/gtobysuvgv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.chenjidiqi.icu/gtojjcoosq.html

[S14] C：枚举
来源：http://hz.jinqigfzy.top/gtdupnokds.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.xingfuxueyuan.xyz/gtmahrqfsz.html

[S15] C：类型转换
来源：http://hz.iojbl.cn/gtligyvyia.html

(double) a / b
来源：http://hz.aizwys.cn/gtrtyixoxo.html

[S16] C：位操作置位
来源：http://hz.shangyingyoupin.top/gtdrtciqpx.html

x |= (1 << 3);
来源：http://hz.yueranfly.top/gtcrlcugzd.html

[S17] C：安全拼接字符串
来源：http://hz.shanyushiyangkeji.top/gtmtjohnsx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.aibaodan.cn/gtrnohfame.html

[S18] C：命令行参数
来源：http://hz.mhx1999.top/gtwfrrffnd.html

int main(int argc, char **argv)
来源：http://hz.tian-w.cn/gtrtqtdqan.html

[S19] C：快速排序
来源：http://hz.hnxiangtu.top/gtvobnzkom.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.dashuyun.cn/gtlbjpuxsu.html

[S20] C：二分查找
来源：http://hz.jqgufenzy.top/gtsvsnyglf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yueranfly.top/gtcsefctff.html

[S21] C：字符类别判断
来源：http://hz.jianghu66.top/gtbkqkvhtq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jqgfzy.top/gtmbljzxmd.html

[S22] C：字符串转数字
来源：http://hz.sysykeji.top/gtnpklscaj.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.daxiang520.top/gtkfxiskyq.html

[S23] C：随机数
来源：http://hz.hnxiangtu.top/gtxzniigeq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.gzhubu.top/gtjevspqby.html

[S24] C：获取本地时间
来源：http://hz.xingfuxueyuan.xyz/gtfnprheyn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.hysaishi.cn/gtolexxofz.html

[S25] C：内存拷贝
来源：http://hz.gogol.net.cn/gteduihejf.html

memcpy(dst, src, n);
来源：http://hz.fengsongda.top/gtrlxqvmqx.html

[S26] C：内存清零
来源：http://hz.dashuyun.cn/gtsihjqghz.html

memset(a, 0, sizeof a);
来源：http://hz.9152youxi.cn/gtszprblvh.html

[S27] C：定义常量
来源：http://hz.yueranfly.top/gtsbbsjzvh.html

const double PI = 3.14159;
来源：http://hz.pengpengdd.cyou/gtodwntxos.html

[S28] C：静态变量
来源：http://hz.zhengqikj.top/gtlvjwjlui.html

static int counter = 0;
来源：http://hz.hysaishi.cn/gtzjpardkg.html

[S29] C：变参函数
来源：http://hz.jqgufenzy.top/gtzjkuugum.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.smart0.xyz/gtzthmtsub.html

[S30] C：头文件保护
来源：http://hz.zhixingplan.top/gtuteompto.html

#ifndef X_H
来源：http://hz.chenjidiqi.icu/gtwzdstimk.html

#define X_H
来源：http://hz.fzhhl.top/gthxsadhmr.html

#endif
来源：http://hz.havefunace.top/gtfnkxxyij.html

[S31] C++：Hello World
来源：http://hz.xingfuxueyuan.xyz/gtnqolgzbv.html

#include <iostream>
来源：http://hz.zycfv.cn/gtikrqhskw.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.shanyushiyangtech.top/gtplomemtl.html

[S32] C++：字符串
来源：http://hz.nwbrower.top/gtotovyzpd.html

std::string s = "hi";  s += "!";
来源：http://hz.yanxiufei.cn/gtauzvmpel.html

[S33] C++：vector 增删
来源：http://hz.wangdashe.top/gtnsjzktuw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.guannengcc.top/gteuvdrpbm.html

[S34] C++：遍历 vector
来源：http://hz.kuanghao11.cn/gtzuaikzps.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yuxming.cn/gteaxyreri.html

[S35] C++：map
来源：http://hz.yanxiufei.cn/gtbjsbnodx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.guannengcc.top/gtigrfabts.html

[S36] C++：unordered_map
来源：http://hz.dianchejie.cn/gtqxjejfbv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shanyushiyangtech.top/gtyncnumui.html

[S37] C++：set
来源：http://hz.yvedp.cn/gtlifjnyrb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.zhongyouzk.top/gtpgkcminf.html

[S38] C++：排序
来源：http://hz.hfpthk.cn/gtssqvvkkz.html

std::sort(v.begin(), v.end());
来源：http://hz.shangyingyoupin.top/gtjhcrzrfi.html


<!-- 参考信息 -->