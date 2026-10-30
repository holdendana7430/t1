代发 wailian999

SHOW INDEX FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxzlzxju.sHtML

[Q73] 查看表状态
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobztehbv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywopmawc.sHtML

[Q74] 强制使用索引
来源：http://blog.fanxiaobao.xyz/Article/details/gfvehdwcv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fanxiaobao.xyz/Article/details/govhfxgsl.sHtML

[Q75] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gusuhnizz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gxlghxcxg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fanxiaobao.xyz/Article/details/gqhljoqpe.sHtML

[Q76] 按天统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmjnnqpw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fanxiaobao.xyz/Article/details/guroyhinh.sHtML

[Q77] 时间加减
来源：http://baike.fanxiaobao.xyz/Article/details/gakbisgir.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fanxiaobao.xyz/Article/details/gjyahvorw.sHtML

[Q78] 当前时间
来源：http://3g.fanxiaobao.xyz/Article/details/gwugvsyqu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fanxiaobao.xyz/Article/details/gricqtvdk.sHtML

[Q79] 字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gwumwyatx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fanxiaobao.xyz/Article/details/gbebzbnhj.sHtML

[Q80] 字符串截取
来源：http://baike.fanxiaobao.xyz/Article/details/gubqzckwp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gtqsuobxl.sHtML

[Q81] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/goffneowb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gonayrkro.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gyeegontp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gzjzznyqh.sHtML

[Q83] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gbejkkcpc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gezbdzptf.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmjxgtgc.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gstjdupzz.sHtML

[Q85] 数值取整
来源：http://www.blog.fanxiaobao.xyz/Article/details/genmjqtnq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykyglgaq.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/geaarycal.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpuikryqw.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fanxiaobao.xyz/Article/details/gmhefiqdc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fanxiaobao.xyz/Article/details/gemmvohmw.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fanxiaobao.xyz/Article/details/ggblrjmrl.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvvwmwvl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/grqphkpto.sHtML

[Q89] 判断表是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/ggajvyynw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/geskxfqbk.sHtML

[Q90] 生成序号列
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhwwvjwv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fanxiaobao.xyz/Article/details/gxtspswcj.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gsuwjzxbk.sHtML

R. Bash 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbduyxek.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gufishhoo.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/gdzqjoxlu.sHtML

#!/usr/bin/env bash
来源：http://wap.fanxiaobao.xyz/Article/details/gmbckbdwz.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwkxijip.sHtML

[R02] 变量赋值与使用
来源：http://blog.fanxiaobao.xyz/Article/details/ggnwtnpua.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpoyabsc.sHtML

[R03] 只读变量
来源：http://read.share.fanxiaobao.xyz/Article/details/glvjungco.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/gghbrwbym.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/gcoztxboa.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fanxiaobao.xyz/Article/details/gjkgwctos.sHtML

[R05] 参数默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gbfmvmxwf.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/grehmgpac.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gduslntcw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgvsivkf.sHtML

[R07] if 判断文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmapjurn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gjoyuxpoh.sHtML

[R08] 数值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gjyrntugi.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/ghavkkfup.sHtML

[R09] 字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gtapesxex.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnqnbuse.sHtML

[R10] 正则匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gaslkzrqb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwtpeapp.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/gmtkufrqf.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpdgokqe.sHtML

start) echo "启动" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtlotpwo.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvauetfm.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gasznvgci.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/gijbdenga.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/gkxfmohcu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/guurpfasg.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffueokeu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdktilcv.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/grssovwuc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbutzgcmm.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvbnbona.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxjaoaga.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmhjkagu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gnhczdkeh.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwamsvrvz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxmsmhph.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/giqtkeuuk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gntiumigw.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gbpvrrpav.sHtML

echo "${#arr[@]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gicffkmgn.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkorlscdi.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gdvxhfgrz.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/ggcdseczj.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqkrzegw.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbpazaqw.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngfrqzny.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/ggncvjbnx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/gkhepiumu.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gfqkxwolx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/gzcbcvder.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdxszwar.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/gjlckghpo.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpinwfhv.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gjljstayt.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gmirwtksp.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gokqxhzrh.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gmoxawgyv.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/gnwchalyx.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gsiqbvqsr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gfhsqnfsh.sHtML

[R30] 函数返回状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gvorjijul.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/gykooeukv.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gerhgltxe.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzielrtyt.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/grsrlvbjv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gaofroxqm.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gmgqrabic.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gdmdszxxb.sHtML

[R34] 退出时清理
来源：http://read.share.fanxiaobao.xyz/Article/details/ggiubbngv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/grhtgtflf.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/glswmwxbc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gfvzvpwyw.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/gxidqwfpl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gmubkvinm.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gbidzeghe.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztgkkwuz.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/gsadljzml.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/geeepmmjz.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/ghixhipbo.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbsrwfir.sHtML

[R40] 追加写日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gsesrusif.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gopxlexze.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/gryfupejo.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gehmpxint.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/ghoqqnvon.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/garkbermd.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/grtsxkvhs.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gkethsewc.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvjdkuru.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/guahoihcc.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gfulzzmcv.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/ggekowzhw.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/gxuuiczkl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnypukgd.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqryeduw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrelapga.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gabskautu.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gkntgttse.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/grdkybbvu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/gjwwptekk.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/gfqqogpkb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/grefejdso.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnwicaca.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gluutvtej.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gbqgzdqug.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvqjqsfu.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gqdnhoerd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/gnvvrdwqg.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gioqjzctb.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdffdlbk.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmpdnemj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/gjxlsjiev.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgeuamep.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdlxevyk.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggspbbmed.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/gehukitwi.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqnminkt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/galoiamxb.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/ggwksgsgv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gchqhmdvv.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwsdpklt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/gogdotmxo.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gvdqjgehf.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjuugemj.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/gibbkglvv.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gytjigeuw.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gjplhaekn.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gxsqoeplm.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxbuzrec.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrjtixug.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujfemqle.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gfrmrimgh.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gpihlnefs.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gueoquflu.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/gpqmthfin.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/gsnbjjyje.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqbepmri.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gbisyxbsc.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gskioargq.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/geymkzneg.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkshfurk.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/ghzfnbeed.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gnzkupwrk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/ggybziejx.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gxsyewtkf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gqsvaukbh.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gemqdpdvd.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/grdoztsap.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geeeccuoe.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gldqvxlwr.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gistqkmgz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/gsartwljp.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdayhybd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gtelbiplv.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/gwocskjoi.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/gtixtvwnk.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/grkztlqiv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/gxuiyafxw.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gciziuapj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gyvwvtlnh.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/guefjaeff.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnfmdkqt.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gtwreybbw.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzfdhcdl.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdffggykd.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/glcisunsy.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrllizxx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/gruikdewe.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/ggfrzuzmc.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/gcriorvtz.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gyemkcppg.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcalldcii.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/grnpqgxjv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmlygujc.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhaqwghp.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwhngnlh.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfndqpmi.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhoezbyr.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gzogjbxqu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnwujfmp.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbqxscyc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/gztewcgzj.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrkqqwnu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gmyfyqrpk.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/gtprowwjq.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhmvckjt.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjsnwuwh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmwjbhpc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gpqlufcut.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslbcvkmh.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/geaobgfsd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gkrqmimds.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/ggpwvwnxq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkunjusgz.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gmduzuehd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvgbdwfv.sHtML

[S15] C：类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwynouwb.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gkzphmauk.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/gpeucsqms.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmsbezst.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gvifeojnz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gvwltjmmi.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gkcmbssec.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyltrhqxf.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjbqjtzd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfvjhklr.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gldurhekr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/garzjieto.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvotfofu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/gklevqgrl.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlcbswme.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/glzfffhfe.sHtML

[S23] C：随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfflicscm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/ggloyrhgw.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmvzwobh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gjrrnkxtw.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgwasgsl.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/gyybtgicq.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/gwoypkuuw.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbaaxmjar.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/genwyjekc.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejpqplpl.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkhukltej.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/glpvfyxxk.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/gyqgfnwic.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohfsdudr.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxpvqtit.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gdmbovzou.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gipkzyfwt.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/ggffdyugr.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gascycajm.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtukkzkf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gkxaazlww.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlzxpfoj.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gtcsodquj.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/grvwgyhqz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/guedvozbi.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdawiolb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkgpdivs.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/gzihimjus.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkonzphma.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdcznsai.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxeincfd.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/ggmsudvgj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajodmszx.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrpriwva.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gppifebho.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gsntfdeis.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkycsmmw.sHtML

[S40] C++：查找元素
来源：http://3g.fanxiaobao.xyz/Article/details/gxnauznkz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gwhaekxan.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihnkqouk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdzioipm.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/gsoxhubes.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxikwjlj.sHtML


<!-- 参考信息 -->