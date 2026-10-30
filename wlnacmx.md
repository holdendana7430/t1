代发 wailian999

ANALYZE TABLE users;
来源：http://www.m.share.fehbvm.com/Article/details/gfcjvenbd.sHtML

[Q71] 查看建表语句
来源：http://m.share.fehbvm.com/Article/details/gvxhpunrl.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.hesvh.cn/Article/details/gzqouoymo.sHtML

[Q72] 查看索引
来源：http://wap.zdbjq.cn/Article/details/gifbznjcw.sHtML

SHOW INDEX FROM users;
来源：http://www.share.zdbjq.cn/Article/details/grlvdmukp.sHtML

[Q73] 查看表状态
来源：http://read.share.hesvh.cn/Article/details/gmmizzbaf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gyteloczm.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.zdbjq.cn/Article/details/gyarekftg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.zdbjq.cn/Article/details/gprrqgtwc.sHtML

[Q75] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gutvqnyjq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gzlrpwmtv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.zdbjq.cn/Article/details/gftmgnhnv.sHtML

[Q76] 按天统计
来源：http://www.blog.zdbjq.cn/Article/details/gzspaecxd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fehbvm.com/Article/details/gdtaypimt.sHtML

[Q77] 时间加减
来源：http://mobile.hesvh.cn/Article/details/gnqnvpdsh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.hesvh.cn/Article/details/grkcgwhbm.sHtML

[Q78] 当前时间
来源：http://3g.fehbvm.com/Article/details/gzumbfmje.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fehbvm.com/Article/details/gybxwsuug.sHtML

[Q79] 字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gtjqqkigf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.hesvh.cn/Article/details/gbthdrynw.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fehbvm.com/Article/details/gaumkkjmw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gohozmzpb.sHtML

[Q81] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gnrcahkgp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gvjawhlvz.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.zdbjq.cn/Article/details/gcemcicen.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gsnsfmvhw.sHtML

[Q83] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gppxrqiwh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gjxssbcge.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fehbvm.com/Article/details/gogzeycnn.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gwehlkbyd.sHtML

[Q85] 数值取整
来源：http://3g.zdbjq.cn/Article/details/gmhtrfoph.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.hesvh.cn/Article/details/gzdyblmlf.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fehbvm.com/Article/details/getuaqwvr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fehbvm.com/Article/details/gmxidepwy.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fehbvm.com/Article/details/gohkldhym.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fehbvm.com/Article/details/gdyrfifry.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.hesvh.cn/Article/details/ggfgaqhwx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.zdbjq.cn/Article/details/geukeljbu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gvmgcivki.sHtML

[Q89] 判断表是否存在
来源：http://read.share.zdbjq.cn/Article/details/gfsvcggng.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.zdbjq.cn/Article/details/ghurffdcl.sHtML

[Q90] 生成序号列
来源：http://3g.fehbvm.com/Article/details/gbuvjqcow.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.zdbjq.cn/Article/details/gjxamzjvn.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gtxeeapgv.sHtML

R. Bash 专题
来源：http://blog.fehbvm.com/Article/details/gtlqnyrif.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gemibonyz.sHtML

[R01] shebang 与严格模式
来源：http://www.share.hesvh.cn/Article/details/gviczheyf.sHtML

#!/usr/bin/env bash
来源：http://blog.fehbvm.com/Article/details/gyqmmsqyj.sHtML

set -euo pipefail
来源：http://baike.fehbvm.com/Article/details/grpgnjwud.sHtML

[R02] 变量赋值与使用
来源：http://blog.fehbvm.com/Article/details/gxlartvab.sHtML

name="Tom"; echo "$name"
来源：http://read.share.zdbjq.cn/Article/details/ggzzzddnl.sHtML

[R03] 只读变量
来源：http://blog.hesvh.cn/Article/details/gamfsgnrq.sHtML

readonly PI=3.14
来源：http://www.m.share.fehbvm.com/Article/details/gpecuviyi.sHtML

[R04] 位置参数
来源：http://m.share.zdbjq.cn/Article/details/gyhgmysof.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.hesvh.cn/Article/details/ghaplvubo.sHtML

[R05] 参数默认值
来源：http://blog.fehbvm.com/Article/details/gvlasdbdd.sHtML

name="${1:-default}"
来源：http://www.blog.zdbjq.cn/Article/details/gyljnyuuy.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fehbvm.com/Article/details/gasppxpim.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gsqmdwyor.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/gayohtdfx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fehbvm.com/Article/details/grwcmgelf.sHtML

[R08] 数值比较
来源：http://baike.hesvh.cn/Article/details/ggsgfdqdp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.zdbjq.cn/Article/details/gbrwkayac.sHtML

[R09] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gpetnpjns.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.zdbjq.cn/Article/details/gerflkris.sHtML

[R10] 正则匹配
来源：http://www.blog.hesvh.cn/Article/details/gpjuugbqp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fehbvm.com/Article/details/ggevrzjux.sHtML

[R11] case 多分支
来源：http://baike.hesvh.cn/Article/details/gixfvzste.sHtML

case "$1" in
来源：http://mobile.zdbjq.cn/Article/details/gcnfuyedk.sHtML

start) echo "启动" ;;
来源：http://m.share.hesvh.cn/Article/details/gvsydzkyi.sHtML

stop)  echo "停止" ;;
来源：http://baike.fehbvm.com/Article/details/gkbpddxke.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gfagqpzpu.sHtML

esac
来源：http://wap.fehbvm.com/Article/details/gfmxnbnic.sHtML

[R12] for 遍历文件
来源：http://read.share.fehbvm.com/Article/details/gvrosbwxp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.hesvh.cn/Article/details/gmqxnnqbd.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/ghvdexxuq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/guuhvizrj.sHtML

[R14] C 风格 for
来源：http://read.share.fehbvm.com/Article/details/gknjnjhqg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gxmhcvfsq.sHtML

[R15] while 逐行读文件
来源：http://www.share.hesvh.cn/Article/details/graogoigp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fehbvm.com/Article/details/gibmgjiwm.sHtML

[R16] until 等待条件
来源：http://wap.zdbjq.cn/Article/details/gdgtwruab.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gjunytzll.sHtML

[R17] 数组定义与取值
来源：http://3g.zdbjq.cn/Article/details/gotmnlolq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.hesvh.cn/Article/details/gpkfhtzjj.sHtML

[R18] 遍历数组
来源：http://blog.fehbvm.com/Article/details/gpdvvlqcl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.hesvh.cn/Article/details/ghnbivmye.sHtML

[R19] 数组长度
来源：http://blog.hesvh.cn/Article/details/ggpgpygfi.sHtML

echo "${#arr[@]}"
来源：http://wap.hesvh.cn/Article/details/gyfzdbpor.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.zdbjq.cn/Article/details/gcvddmwdu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.hesvh.cn/Article/details/goddxddyk.sHtML

[R21] 字符串长度
来源：http://baike.fehbvm.com/Article/details/gygjfbech.sHtML

echo "${#s}"
来源：http://mobile.zdbjq.cn/Article/details/gjrtepvst.sHtML

[R22] 截取子串
来源：http://mobile.fehbvm.com/Article/details/gpwhmjckg.sHtML

echo "${s:0:5}"
来源：http://www.share.hesvh.cn/Article/details/gdfcyfclx.sHtML

[R23] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gcfaetkvg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fehbvm.com/Article/details/gcvgekxlg.sHtML

[R24] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gyrrtyusm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.hesvh.cn/Article/details/gpcgjwcec.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.hesvh.cn/Article/details/gereutggq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fehbvm.com/Article/details/gsmqshvva.sHtML

[R26] 命令替换
来源：http://www.blog.hesvh.cn/Article/details/gevzfamlt.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/gnhyibjye.sHtML

[R27] 算术展开
来源：http://read.share.hesvh.cn/Article/details/gthqsdmer.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fehbvm.com/Article/details/gslabsbln.sHtML

[R28] 浮点运算
来源：http://m.share.zdbjq.cn/Article/details/gwingjvub.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.zdbjq.cn/Article/details/gvkfokhec.sHtML

[R29] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gceskubdb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.hesvh.cn/Article/details/gtyzhafwp.sHtML

[R30] 函数返回状态码
来源：http://wap.fehbvm.com/Article/details/gyzqdntdd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.hesvh.cn/Article/details/gcfjpjnzz.sHtML

[R31] 局部变量
来源：http://m.share.hesvh.cn/Article/details/gazjvxigv.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.hesvh.cn/Article/details/gkecukaiv.sHtML

[R32] 参数个数校验
来源：http://read.share.hesvh.cn/Article/details/gvtkfwejw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gfanvajns.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.zdbjq.cn/Article/details/gtexytzty.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.hesvh.cn/Article/details/gqnfjxpbs.sHtML

[R34] 退出时清理
来源：http://blog.zdbjq.cn/Article/details/gaxhscauy.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gdlmjtibf.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.hesvh.cn/Article/details/gkeraidco.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.zdbjq.cn/Article/details/gobperndk.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.hesvh.cn/Article/details/gomwbykzr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.hesvh.cn/Article/details/giefqvoir.sHtML

[R37] 把输出赋给变量
来源：http://baike.zdbjq.cn/Article/details/gsdntfebz.sHtML

files=$(ls -1)
来源：http://www.share.hesvh.cn/Article/details/gakwbwagm.sHtML

[R38] 管道串联
来源：http://read.share.fehbvm.com/Article/details/glzakzeeb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fehbvm.com/Article/details/gbggaqxlq.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.hesvh.cn/Article/details/gqurceokv.sHtML

cmd > out.log 2>&1
来源：http://wap.zdbjq.cn/Article/details/gafmjrdnz.sHtML

[R40] 追加写日志
来源：http://www.blog.hesvh.cn/Article/details/gztqzhbcm.sHtML

echo "log" >> out.log
来源：http://baike.hesvh.cn/Article/details/gzflmolct.sHtML

[R41] 丢弃输出
来源：http://baike.fehbvm.com/Article/details/glolooujl.sHtML

cmd >/dev/null 2>&1
来源：http://3g.hesvh.cn/Article/details/glsrbrxej.sHtML

[R42] 输入重定向
来源：http://www.m.share.fehbvm.com/Article/details/gcezctwuq.sHtML

wc -l < a.txt
来源：http://www.blog.hesvh.cn/Article/details/gwvbmxgiv.sHtML

[R43] 按名字查找文件
来源：http://3g.zdbjq.cn/Article/details/gibfatlcm.sHtML

find . -name "*.log" -type f
来源：http://mobile.zdbjq.cn/Article/details/gmkhmrqqi.sHtML

[R44] 按修改时间查找
来源：http://blog.zdbjq.cn/Article/details/gfackdpjs.sHtML

find . -mtime -7 -type f
来源：http://mobile.hesvh.cn/Article/details/gemndudlt.sHtML

[R45] 批量删除
来源：http://www.blog.hesvh.cn/Article/details/gqomrriuv.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.zdbjq.cn/Article/details/gcipqluoc.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/gkxjcptpp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.zdbjq.cn/Article/details/gjlrlfloq.sHtML

[R47] sed 单行替换
来源：http://mobile.zdbjq.cn/Article/details/gsfvjhial.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fehbvm.com/Article/details/gtfomzdju.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/gmghvhnol.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.hesvh.cn/Article/details/ghsyinagq.sHtML

[R49] awk 带条件
来源：http://wap.zdbjq.cn/Article/details/glcnpgwcj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.zdbjq.cn/Article/details/gqtnxrtkm.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/gvbxqkczc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/glakxwlqc.sHtML

[R51] 排序去重取前几
来源：http://www.share.hesvh.cn/Article/details/gjcgvzeby.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.hesvh.cn/Article/details/gxisjwsrm.sHtML

[R52] 统计行数
来源：http://www.blog.hesvh.cn/Article/details/goickywvl.sHtML

wc -l a.txt
来源：http://3g.fehbvm.com/Article/details/giviixfmt.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.hesvh.cn/Article/details/gcarlngmr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.zdbjq.cn/Article/details/gxdtbesix.sHtML

[R54] 比较两个文件
来源：http://www.blog.fehbvm.com/Article/details/gtiutflkn.sHtML

diff a.txt b.txt
来源：http://read.share.hesvh.cn/Article/details/gunrmqyny.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/glhnciwof.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.hesvh.cn/Article/details/gvjsfoxqu.sHtML

[R56] 远程拷贝
来源：http://read.share.fehbvm.com/Article/details/grormcnvw.sHtML

scp file user@host:/path/
来源：http://www.share.zdbjq.cn/Article/details/gyzbpzdzi.sHtML

[R57] 远程执行命令
来源：http://blog.zdbjq.cn/Article/details/gtdtjobzk.sHtML

ssh user@host 'uptime'
来源：http://read.share.hesvh.cn/Article/details/guoitwrjn.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/gysgpcdfa.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fehbvm.com/Article/details/ghwesdyjj.sHtML

[R59] 发 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gxuwktang.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.hesvh.cn/Article/details/gutoubunv.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/ghvwxxkva.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fehbvm.com/Article/details/gqyxkddix.sHtML

[R61] 磁盘占用
来源：http://www.blog.zdbjq.cn/Article/details/gfqpqetrr.sHtML

df -h;  du -sh *
来源：http://3g.zdbjq.cn/Article/details/gscjtfoom.sHtML

[R62] 找最占空间的文件
来源：http://m.share.zdbjq.cn/Article/details/gfgzrxwos.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fehbvm.com/Article/details/geychpcqr.sHtML

[R63] 内存与进程
来源：http://www.share.zdbjq.cn/Article/details/gjuhruhnx.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fehbvm.com/Article/details/gjihqbbio.sHtML

[R64] 结束进程
来源：http://wap.fehbvm.com/Article/details/guqpqzylr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.zdbjq.cn/Article/details/gfzqrflba.sHtML

[R65] 查看端口占用
来源：http://m.share.fehbvm.com/Article/details/gahoggmzn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.hesvh.cn/Article/details/gqdtlpwam.sHtML

[R66] 定时任务
来源：http://mobile.zdbjq.cn/Article/details/gbzpbyzqg.sHtML

crontab -e;  crontab -l
来源：http://baike.hesvh.cn/Article/details/gzzlkqdsa.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.hesvh.cn/Article/details/gofnjvxpt.sHtML

openssl rand -hex 16
来源：http://mobile.hesvh.cn/Article/details/gaocpgfiz.sHtML

[R68] 计算文件校验值
来源：http://read.share.fehbvm.com/Article/details/gpbhrkrnj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.hesvh.cn/Article/details/gftxdknng.sHtML

[R69] 生成随机密码
来源：http://read.share.zdbjq.cn/Article/details/guwmwamgb.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/gwueibijo.sHtML

[R70] 时间戳与互转
来源：http://blog.fehbvm.com/Article/details/gkdsnhvgo.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/gkiuusuxx.sHtML

[R71] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/grhkdihua.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fehbvm.com/Article/details/gpfgzccjx.sHtML

[R72] 等待端口就绪
来源：http://baike.zdbjq.cn/Article/details/gnqmuttfx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gmnyzfxfp.sHtML

[R73] 分割大日志
来源：http://mobile.hesvh.cn/Article/details/gommuaxbx.sHtML

split -l 1000 big.log part_
来源：http://wap.fehbvm.com/Article/details/gwgqoardl.sHtML

[R74] 批量重命名
来源：http://m.share.fehbvm.com/Article/details/granzupmx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.hesvh.cn/Article/details/goushujjo.sHtML

[R75] 导出环境变量
来源：http://baike.zdbjq.cn/Article/details/gvzzhixdp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.zdbjq.cn/Article/details/gqqribqtw.sHtML

[R76] 使用临时文件
来源：http://baike.zdbjq.cn/Article/details/guekcndfo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gegtoqdng.sHtML

[R77] 读取用户输入
来源：http://www.share.fehbvm.com/Article/details/gyftajley.sHtML

read -rp "请输入: " ans
来源：http://www.share.hesvh.cn/Article/details/gipybnhtl.sHtML

[R78] 交互式菜单
来源：http://read.share.zdbjq.cn/Article/details/ggngpuiqk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/gvhmjvfna.sHtML

[R79] 解析命令行选项
来源：http://blog.zdbjq.cn/Article/details/gbtbrjsit.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.hesvh.cn/Article/details/grpzfvwqu.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.zdbjq.cn/Article/details/gwkmmfaud.sHtML

time ./run.sh
来源：http://wap.fehbvm.com/Article/details/ggfktxvcv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gsyckerzf.sHtML

S. C / C++ 专题
来源：http://blog.fehbvm.com/Article/details/gkobeynff.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwakduykt.sHtML

[S01] C：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gfihtpppi.sHtML

#include <stdio.h>
来源：http://read.share.hesvh.cn/Article/details/gdsctmpqr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.zdbjq.cn/Article/details/gkbudnxnq.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fehbvm.com/Article/details/gsfsknwer.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/gxspgyknp.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/gkmjezsex.sHtML

int x; scanf("%d", &x);
来源：http://blog.hesvh.cn/Article/details/gdvfjowbz.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/ggxtqbdwz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.hesvh.cn/Article/details/gfivpfkvj.sHtML

[S05] C：字符串长度
来源：http://m.share.zdbjq.cn/Article/details/getyfdtbk.sHtML

strlen(s)
来源：http://www.m.share.fehbvm.com/Article/details/gufuhdklw.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/gzetwuifz.sHtML

strcmp(a, b) == 0
来源：http://www.share.fehbvm.com/Article/details/ghjizeqeq.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fehbvm.com/Article/details/gbpomzldl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.hesvh.cn/Article/details/gneelghvp.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/gvbgnoejg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.hesvh.cn/Article/details/gltuedxzn.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.zdbjq.cn/Article/details/gtzrmfulv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/gghjaqipo.sHtML

[S10] C：指针与解引用
来源：http://mobile.zdbjq.cn/Article/details/gucisgngu.sHtML

int *p = &a;  *p = 5;
来源：http://blog.hesvh.cn/Article/details/gedbsysdo.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gtbgjnviz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/gjjmsdeih.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fehbvm.com/Article/details/gjzmvqlhw.sHtML

fclose(f);
来源：http://wap.hesvh.cn/Article/details/ggrmphhlw.sHtML

[S12] C：写文件
来源：http://www.share.zdbjq.cn/Article/details/gxzpflday.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/getfkixns.sHtML

[S13] C：宏定义
来源：http://www.m.share.fehbvm.com/Article/details/gtiolprfu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.zdbjq.cn/Article/details/gsucrlfkv.sHtML

[S14] C：枚举
来源：http://www.share.zdbjq.cn/Article/details/gtbfrhdpk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fehbvm.com/Article/details/gdiqdphfx.sHtML

[S15] C：类型转换
来源：http://www.share.fehbvm.com/Article/details/gyzluqkyo.sHtML

(double) a / b
来源：http://read.share.zdbjq.cn/Article/details/gnavdrevq.sHtML

[S16] C：位操作置位
来源：http://read.share.hesvh.cn/Article/details/gnuhyvqxi.sHtML

x |= (1 << 3);
来源：http://www.m.share.hesvh.cn/Article/details/gaceufikj.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gtaqktlqo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/gxmvjmetc.sHtML

[S18] C：命令行参数
来源：http://3g.hesvh.cn/Article/details/gsgjkenlh.sHtML

int main(int argc, char **argv)
来源：http://blog.hesvh.cn/Article/details/grggnhdcf.sHtML

[S19] C：快速排序
来源：http://blog.hesvh.cn/Article/details/gmxvalapx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gwwlbzlrg.sHtML

[S20] C：二分查找
来源：http://baike.hesvh.cn/Article/details/ggeonbeox.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gegtdnhfq.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.hesvh.cn/Article/details/gjdvyseml.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fehbvm.com/Article/details/gjldbpsac.sHtML

[S22] C：字符串转数字
来源：http://blog.zdbjq.cn/Article/details/ggyayfhzc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.zdbjq.cn/Article/details/gupkksjux.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/gelnjzfjn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fehbvm.com/Article/details/guqjssgst.sHtML

[S24] C：获取本地时间
来源：http://3g.fehbvm.com/Article/details/gavovwoqv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fehbvm.com/Article/details/gmeetsmgo.sHtML

[S25] C：内存拷贝
来源：http://baike.hesvh.cn/Article/details/gigsfhdzc.sHtML

memcpy(dst, src, n);
来源：http://read.share.fehbvm.com/Article/details/gbcdtdpqr.sHtML

[S26] C：内存清零
来源：http://www.m.share.hesvh.cn/Article/details/gorfullkg.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fehbvm.com/Article/details/gqzdjxqaz.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/gdphuunor.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gfnhrragx.sHtML

[S28] C：静态变量
来源：http://mobile.zdbjq.cn/Article/details/gyfurkung.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/grzwweduv.sHtML

[S29] C：变参函数
来源：http://3g.hesvh.cn/Article/details/gwhojnulh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fehbvm.com/Article/details/gxloffwoc.sHtML

[S30] C：头文件保护
来源：http://read.share.zdbjq.cn/Article/details/guzsyltko.sHtML

#ifndef X_H
来源：http://www.blog.zdbjq.cn/Article/details/gloadznqx.sHtML

#define X_H
来源：http://www.blog.hesvh.cn/Article/details/gdbqhgjmr.sHtML

#endif
来源：http://baike.fehbvm.com/Article/details/gxsftzsqu.sHtML

[S31] C++：Hello World
来源：http://www.share.hesvh.cn/Article/details/gvixhznkl.sHtML

#include <iostream>
来源：http://www.m.share.hesvh.cn/Article/details/gwegnxosx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.zdbjq.cn/Article/details/gshklhfvc.sHtML

[S32] C++：字符串
来源：http://www.share.zdbjq.cn/Article/details/gundxhlvw.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.hesvh.cn/Article/details/grzmffhen.sHtML

[S33] C++：vector 增删
来源：http://www.blog.zdbjq.cn/Article/details/ggwyboegf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/gyxqsnzaz.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fehbvm.com/Article/details/gmjxljvoi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fehbvm.com/Article/details/gwkowqzvv.sHtML

[S35] C++：map
来源：http://www.share.fehbvm.com/Article/details/ggbblzitg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gxovcnrhv.sHtML

[S36] C++：unordered_map
来源：http://blog.fehbvm.com/Article/details/glyibdxhn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gdbvyubfy.sHtML

[S37] C++：set
来源：http://www.blog.hesvh.cn/Article/details/gwwyurtpa.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gsqplheyc.sHtML

[S38] C++：排序
来源：http://read.share.fehbvm.com/Article/details/gzjiodutb.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.hesvh.cn/Article/details/gkhmthrab.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.zdbjq.cn/Article/details/gprzkeksn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fehbvm.com/Article/details/ghqswxgfz.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/gngkifdvm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fehbvm.com/Article/details/gzuvcdqua.sHtML


<!-- 参考信息 -->