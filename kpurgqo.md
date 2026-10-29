代发 wailian999

ANALYZE TABLE users;
来源：http://www.m.share.fehbvm.com/Article/details/govxqkbbl.sHtML

[Q71] 查看建表语句
来源：http://mobile.zdbjq.cn/Article/details/gazdoejob.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.zdbjq.cn/Article/details/gnoevipkc.sHtML

[Q72] 查看索引
来源：http://www.m.share.fehbvm.com/Article/details/gyqtbzlcu.sHtML

SHOW INDEX FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gibfpztwb.sHtML

[Q73] 查看表状态
来源：http://www.share.fehbvm.com/Article/details/glasbactv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.zdbjq.cn/Article/details/gochsntij.sHtML

[Q74] 强制使用索引
来源：http://wap.hesvh.cn/Article/details/gglnhvbby.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fehbvm.com/Article/details/gbifpwwhr.sHtML

[Q75] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gozwrhlkh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gmzaqodyu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.zdbjq.cn/Article/details/gqputpilb.sHtML

[Q76] 按天统计
来源：http://wap.fehbvm.com/Article/details/gmcimjpcr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.zdbjq.cn/Article/details/gijflbsys.sHtML

[Q77] 时间加减
来源：http://www.share.hesvh.cn/Article/details/geblzhknc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.zdbjq.cn/Article/details/gwvhhnbtq.sHtML

[Q78] 当前时间
来源：http://www.m.share.hesvh.cn/Article/details/gpdzbosba.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.hesvh.cn/Article/details/gbwvygnog.sHtML

[Q79] 字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gqkmbcdxo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.hesvh.cn/Article/details/goinqzpaz.sHtML

[Q80] 字符串截取
来源：http://wap.hesvh.cn/Article/details/gzysmnmuf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gnhptrjnh.sHtML

[Q81] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/guugaptsn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fehbvm.com/Article/details/gyedepzss.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.zdbjq.cn/Article/details/gyupffric.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gyncnzuxk.sHtML

[Q83] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/guogyppsx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gwppbvsto.sHtML

[Q84] 去除首尾空格
来源：http://wap.fehbvm.com/Article/details/gonyhtzwc.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gjehiozin.sHtML

[Q85] 数值取整
来源：http://www.share.fehbvm.com/Article/details/ggrllocuu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.hesvh.cn/Article/details/gjtzbhucm.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.hesvh.cn/Article/details/gjfaumbns.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.hesvh.cn/Article/details/gmxyjmkyv.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.zdbjq.cn/Article/details/gjrvsyvgf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.zdbjq.cn/Article/details/gyjnvbilr.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.zdbjq.cn/Article/details/gbqlgctsz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.zdbjq.cn/Article/details/gqtnrmbqu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.hesvh.cn/Article/details/ghrccdacz.sHtML

[Q89] 判断表是否存在
来源：http://3g.fehbvm.com/Article/details/ggcweptwq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.zdbjq.cn/Article/details/gajzrdeqe.sHtML

[Q90] 生成序号列
来源：http://www.m.share.zdbjq.cn/Article/details/galyzunjb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.hesvh.cn/Article/details/gksqhlzfu.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmyhbnzzq.sHtML

R. Bash 专题
来源：http://www.share.hesvh.cn/Article/details/gtyxglnbq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gehpcstsp.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fehbvm.com/Article/details/gyuawlfdd.sHtML

#!/usr/bin/env bash
来源：http://baike.zdbjq.cn/Article/details/gsawwdgmz.sHtML

set -euo pipefail
来源：http://mobile.hesvh.cn/Article/details/goialdboi.sHtML

[R02] 变量赋值与使用
来源：http://mobile.hesvh.cn/Article/details/geirrdcwx.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fehbvm.com/Article/details/garqowfeh.sHtML

[R03] 只读变量
来源：http://baike.fehbvm.com/Article/details/gjzghftyy.sHtML

readonly PI=3.14
来源：http://m.share.hesvh.cn/Article/details/gjbqrdutg.sHtML

[R04] 位置参数
来源：http://m.share.hesvh.cn/Article/details/gtjuishde.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.zdbjq.cn/Article/details/gdkhahrnd.sHtML

[R05] 参数默认值
来源：http://blog.hesvh.cn/Article/details/gzevvdwrg.sHtML

name="${1:-default}"
来源：http://3g.hesvh.cn/Article/details/glcfytbal.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gsazmloqz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gimdflhlc.sHtML

[R07] if 判断文件
来源：http://read.share.hesvh.cn/Article/details/gjikrrquq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.zdbjq.cn/Article/details/gaetdigin.sHtML

[R08] 数值比较
来源：http://3g.fehbvm.com/Article/details/gikpepfwk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.zdbjq.cn/Article/details/gnujuhzud.sHtML

[R09] 字符串比较
来源：http://blog.zdbjq.cn/Article/details/gnoesrlts.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fehbvm.com/Article/details/gbzydtbyn.sHtML

[R10] 正则匹配
来源：http://www.share.zdbjq.cn/Article/details/gmwgzxmgs.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fehbvm.com/Article/details/gpllwzjjo.sHtML

[R11] case 多分支
来源：http://blog.hesvh.cn/Article/details/gyhabffhr.sHtML

case "$1" in
来源：http://3g.fehbvm.com/Article/details/giwcoyevb.sHtML

start) echo "启动" ;;
来源：http://3g.fehbvm.com/Article/details/gccciqjae.sHtML

stop)  echo "停止" ;;
来源：http://m.share.hesvh.cn/Article/details/grfakrzpy.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.zdbjq.cn/Article/details/ggfpnqkdq.sHtML

esac
来源：http://read.share.fehbvm.com/Article/details/grglvkrho.sHtML

[R12] for 遍历文件
来源：http://wap.zdbjq.cn/Article/details/gnvcvyxix.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.hesvh.cn/Article/details/gutuqpjxl.sHtML

[R13] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/gaidsrxdh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gfxcmxtoz.sHtML

[R14] C 风格 for
来源：http://wap.zdbjq.cn/Article/details/grgtkgbfo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gpxafxyau.sHtML

[R15] while 逐行读文件
来源：http://blog.fehbvm.com/Article/details/gftxtxrcj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.hesvh.cn/Article/details/guzyufjme.sHtML

[R16] until 等待条件
来源：http://mobile.zdbjq.cn/Article/details/gbsdmrari.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gowjbclou.sHtML

[R17] 数组定义与取值
来源：http://blog.hesvh.cn/Article/details/gzfbacpge.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fehbvm.com/Article/details/gvrcvdpbn.sHtML

[R18] 遍历数组
来源：http://wap.fehbvm.com/Article/details/guqbbbdpz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.hesvh.cn/Article/details/gdnzfgjvo.sHtML

[R19] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/gwugkpked.sHtML

echo "${#arr[@]}"
来源：http://www.share.zdbjq.cn/Article/details/ghggkunuk.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fehbvm.com/Article/details/gdwgjroll.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.hesvh.cn/Article/details/gzgezmxbi.sHtML

[R21] 字符串长度
来源：http://read.share.hesvh.cn/Article/details/glvjtifid.sHtML

echo "${#s}"
来源：http://www.m.share.zdbjq.cn/Article/details/gvedubnhb.sHtML

[R22] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gjlckyjon.sHtML

echo "${s:0:5}"
来源：http://mobile.zdbjq.cn/Article/details/gykgswwdi.sHtML

[R23] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gjokwviuv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.hesvh.cn/Article/details/ggzdwbdtb.sHtML

[R24] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gofvhyqyn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.zdbjq.cn/Article/details/gtujougbq.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fehbvm.com/Article/details/gtwxkspmf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.hesvh.cn/Article/details/gpmufinvz.sHtML

[R26] 命令替换
来源：http://www.blog.zdbjq.cn/Article/details/gocbgffym.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.zdbjq.cn/Article/details/grffoxlth.sHtML

[R27] 算术展开
来源：http://www.m.share.fehbvm.com/Article/details/gttyneygi.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.zdbjq.cn/Article/details/godcppdye.sHtML

[R28] 浮点运算
来源：http://read.share.fehbvm.com/Article/details/ghfadmayq.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.zdbjq.cn/Article/details/gpowdpfkf.sHtML

[R29] 定义函数
来源：http://3g.hesvh.cn/Article/details/gkbqojpqx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fehbvm.com/Article/details/gkywnxlbc.sHtML

[R30] 函数返回状态码
来源：http://blog.zdbjq.cn/Article/details/gkeqapgyj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.hesvh.cn/Article/details/gbrccqzjc.sHtML

[R31] 局部变量
来源：http://www.blog.fehbvm.com/Article/details/gzzaoznqi.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.zdbjq.cn/Article/details/gvlraxigj.sHtML

[R32] 参数个数校验
来源：http://baike.zdbjq.cn/Article/details/ggwneksog.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/giqeymqas.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fehbvm.com/Article/details/gznknppbl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fehbvm.com/Article/details/gxyctayiz.sHtML

[R34] 退出时清理
来源：http://3g.zdbjq.cn/Article/details/gchhyggev.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gjtyvctpp.sHtML

[R35] 后台执行并等待
来源：http://3g.fehbvm.com/Article/details/gwhowlekp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/gqwsrswiq.sHtML

[R36] 并发执行多个任务
来源：http://mobile.hesvh.cn/Article/details/ghuyygiru.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.zdbjq.cn/Article/details/gjdeemhoc.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fehbvm.com/Article/details/gxgxxyern.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/ghqtabusk.sHtML

[R38] 管道串联
来源：http://3g.zdbjq.cn/Article/details/gduoyiusj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.hesvh.cn/Article/details/gplchlsin.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fehbvm.com/Article/details/gklbtkhzg.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gqtdywsma.sHtML

[R40] 追加写日志
来源：http://read.share.fehbvm.com/Article/details/gesmcntgl.sHtML

echo "log" >> out.log
来源：http://wap.zdbjq.cn/Article/details/gvnivargo.sHtML

[R41] 丢弃输出
来源：http://www.share.hesvh.cn/Article/details/gkciyjhez.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.hesvh.cn/Article/details/gkhvstawv.sHtML

[R42] 输入重定向
来源：http://baike.hesvh.cn/Article/details/gtjpbxkuw.sHtML

wc -l < a.txt
来源：http://www.blog.hesvh.cn/Article/details/gthznllrj.sHtML

[R43] 按名字查找文件
来源：http://m.share.zdbjq.cn/Article/details/gtqpdycvn.sHtML

find . -name "*.log" -type f
来源：http://www.share.hesvh.cn/Article/details/grmzgmqvp.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.hesvh.cn/Article/details/gzjdaxitj.sHtML

find . -mtime -7 -type f
来源：http://mobile.hesvh.cn/Article/details/gkjzbewlw.sHtML

[R45] 批量删除
来源：http://baike.hesvh.cn/Article/details/gvvrwcapz.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fehbvm.com/Article/details/gkknbbjpn.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fehbvm.com/Article/details/gesuomlbw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fehbvm.com/Article/details/gliflwycv.sHtML

[R47] sed 单行替换
来源：http://m.share.fehbvm.com/Article/details/guiqhpuzs.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/gxmvlbaxu.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fehbvm.com/Article/details/gnsupbtwp.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fehbvm.com/Article/details/gkovllecr.sHtML

[R49] awk 带条件
来源：http://read.share.zdbjq.cn/Article/details/gnllkfssb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/gohsyvjmr.sHtML

[R50] awk 求和
来源：http://www.blog.fehbvm.com/Article/details/gewjxurvt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fehbvm.com/Article/details/gzirnidkc.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/gcszahsiw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fehbvm.com/Article/details/gtemgfspf.sHtML

[R52] 统计行数
来源：http://www.m.share.zdbjq.cn/Article/details/gshrhygds.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/gsfozzeaq.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.zdbjq.cn/Article/details/gtuvyrgkz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fehbvm.com/Article/details/gphjghpxc.sHtML

[R54] 比较两个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gaxwedbqw.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gdsxadkcp.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fehbvm.com/Article/details/gpxbiqwck.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.zdbjq.cn/Article/details/gdxqrmacx.sHtML

[R56] 远程拷贝
来源：http://mobile.fehbvm.com/Article/details/gzlyiwmig.sHtML

scp file user@host:/path/
来源：http://3g.zdbjq.cn/Article/details/grmlarzwn.sHtML

[R57] 远程执行命令
来源：http://wap.zdbjq.cn/Article/details/gxjlzacnx.sHtML

ssh user@host 'uptime'
来源：http://baike.zdbjq.cn/Article/details/goclymcbh.sHtML

[R58] 下载文件
来源：http://m.share.hesvh.cn/Article/details/gwfmtbucb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fehbvm.com/Article/details/grhfptgjo.sHtML

[R59] 发 POST JSON
来源：http://blog.fehbvm.com/Article/details/gkookzmbj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.hesvh.cn/Article/details/gcukxvlmk.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/gxrhnybyq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.hesvh.cn/Article/details/gnuxupdjj.sHtML

[R61] 磁盘占用
来源：http://baike.fehbvm.com/Article/details/gpnpbyydw.sHtML

df -h;  du -sh *
来源：http://wap.fehbvm.com/Article/details/gqbmipgmr.sHtML

[R62] 找最占空间的文件
来源：http://m.share.hesvh.cn/Article/details/gmnwxsarq.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.hesvh.cn/Article/details/gftlhpjao.sHtML

[R63] 内存与进程
来源：http://3g.zdbjq.cn/Article/details/gwgbgjdyo.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.hesvh.cn/Article/details/gnitwvqck.sHtML

[R64] 结束进程
来源：http://blog.hesvh.cn/Article/details/glwrxpktr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.zdbjq.cn/Article/details/gfseowhab.sHtML

[R65] 查看端口占用
来源：http://baike.fehbvm.com/Article/details/gezmpsqav.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.zdbjq.cn/Article/details/gwnajaigu.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/getigcoyq.sHtML

crontab -e;  crontab -l
来源：http://blog.zdbjq.cn/Article/details/gtiltulsy.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fehbvm.com/Article/details/gwsdnsoik.sHtML

openssl rand -hex 16
来源：http://www.share.zdbjq.cn/Article/details/godnexpqo.sHtML

[R68] 计算文件校验值
来源：http://www.share.fehbvm.com/Article/details/gfzjgqxko.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gxokdwbbn.sHtML

[R69] 生成随机密码
来源：http://read.share.hesvh.cn/Article/details/gtlepsqmb.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.zdbjq.cn/Article/details/galawyfav.sHtML

[R70] 时间戳与互转
来源：http://m.share.fehbvm.com/Article/details/gbolnryyg.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/gdfehfntz.sHtML

[R71] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gshlfvnxv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fehbvm.com/Article/details/gyqjxialm.sHtML

[R72] 等待端口就绪
来源：http://m.share.fehbvm.com/Article/details/gzuzqyncf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gybhnrsqw.sHtML

[R73] 分割大日志
来源：http://www.share.hesvh.cn/Article/details/gcsqrqhos.sHtML

split -l 1000 big.log part_
来源：http://wap.fehbvm.com/Article/details/ghvdjvegp.sHtML

[R74] 批量重命名
来源：http://read.share.hesvh.cn/Article/details/gyfjiewgu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.hesvh.cn/Article/details/gparotcut.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/gqytfcqcn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.zdbjq.cn/Article/details/gcjtyocte.sHtML

[R76] 使用临时文件
来源：http://wap.fehbvm.com/Article/details/gtbxsbsbb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gqgubximc.sHtML

[R77] 读取用户输入
来源：http://mobile.hesvh.cn/Article/details/grvldljqt.sHtML

read -rp "请输入: " ans
来源：http://mobile.hesvh.cn/Article/details/gbmntvzmf.sHtML

[R78] 交互式菜单
来源：http://mobile.zdbjq.cn/Article/details/gvektwufd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/gvayfficy.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.zdbjq.cn/Article/details/gnpmlvhzu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fehbvm.com/Article/details/gmozyazrr.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/gmedxomhp.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/gdnmrvvmz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfoivrkvc.sHtML

S. C / C++ 专题
来源：http://www.m.share.hesvh.cn/Article/details/gwfzqhyyf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gpaesocbd.sHtML

[S01] C：Hello World
来源：http://m.share.hesvh.cn/Article/details/glgbwmozm.sHtML

#include <stdio.h>
来源：http://www.blog.zdbjq.cn/Article/details/gslmijuxo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.zdbjq.cn/Article/details/gufxosphb.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.hesvh.cn/Article/details/gqkzdrxor.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.zdbjq.cn/Article/details/gtwcqvxdx.sHtML

[S03] C：读入整数
来源：http://mobile.fehbvm.com/Article/details/gonfdarsp.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.hesvh.cn/Article/details/glwvoopyv.sHtML

[S04] C：字符串复制
来源：http://mobile.hesvh.cn/Article/details/gelbumaor.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.zdbjq.cn/Article/details/gdnftnsvz.sHtML

[S05] C：字符串长度
来源：http://mobile.hesvh.cn/Article/details/gtrohqcco.sHtML

strlen(s)
来源：http://www.m.share.hesvh.cn/Article/details/gsagniziy.sHtML

[S06] C：字符串比较
来源：http://m.share.fehbvm.com/Article/details/gbttjltby.sHtML

strcmp(a, b) == 0
来源：http://wap.fehbvm.com/Article/details/gukmokbpn.sHtML

[S07] C：数组遍历求和
来源：http://3g.hesvh.cn/Article/details/gdpuckzrq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.hesvh.cn/Article/details/gqkxbbtcc.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.hesvh.cn/Article/details/gemqjricy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.zdbjq.cn/Article/details/gtkugmjjg.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/gguappvjz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/gdvvbcixw.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gfvffhlgg.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/glwnnjehf.sHtML

[S11] C：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gxlmdaena.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.hesvh.cn/Article/details/grrjfvqoc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gkqzancce.sHtML

fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gcesrioks.sHtML

[S12] C：写文件
来源：http://baike.zdbjq.cn/Article/details/gjzmrlzgj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gninyovcf.sHtML

[S13] C：宏定义
来源：http://www.m.share.hesvh.cn/Article/details/gvevfyjpn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.hesvh.cn/Article/details/gsmwhpodf.sHtML

[S14] C：枚举
来源：http://blog.hesvh.cn/Article/details/gtudkiwpi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.zdbjq.cn/Article/details/gzmbkvanr.sHtML

[S15] C：类型转换
来源：http://wap.hesvh.cn/Article/details/gxldxbhdx.sHtML

(double) a / b
来源：http://baike.hesvh.cn/Article/details/gyudsoifs.sHtML

[S16] C：位操作置位
来源：http://www.share.hesvh.cn/Article/details/gbohjnvhi.sHtML

x |= (1 << 3);
来源：http://3g.hesvh.cn/Article/details/gztuhaobq.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gherzhyyu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.zdbjq.cn/Article/details/giyuusbez.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gnwuaycgw.sHtML

int main(int argc, char **argv)
来源：http://m.share.zdbjq.cn/Article/details/ggzsluear.sHtML

[S19] C：快速排序
来源：http://www.share.zdbjq.cn/Article/details/gibauiain.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gdnpylzgd.sHtML

[S20] C：二分查找
来源：http://read.share.zdbjq.cn/Article/details/gfrxtcpft.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/ghzxrhtdj.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.hesvh.cn/Article/details/gryjbxlrn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.hesvh.cn/Article/details/gwqusyhxj.sHtML

[S22] C：字符串转数字
来源：http://baike.fehbvm.com/Article/details/ggdqnfueb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/gtbyvhawy.sHtML

[S23] C：随机数
来源：http://baike.hesvh.cn/Article/details/gezpftovr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.hesvh.cn/Article/details/gfepwlgld.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.hesvh.cn/Article/details/gwmjshaeb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fehbvm.com/Article/details/gospsksbu.sHtML

[S25] C：内存拷贝
来源：http://mobile.hesvh.cn/Article/details/gslrnuenu.sHtML

memcpy(dst, src, n);
来源：http://m.share.hesvh.cn/Article/details/gygwpwhye.sHtML

[S26] C：内存清零
来源：http://www.blog.fehbvm.com/Article/details/gugautyvf.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.zdbjq.cn/Article/details/galzjhlut.sHtML

[S27] C：定义常量
来源：http://mobile.fehbvm.com/Article/details/gampiotdp.sHtML

const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gmcpmprhq.sHtML

[S28] C：静态变量
来源：http://www.m.share.hesvh.cn/Article/details/gfavvqbqy.sHtML

static int counter = 0;
来源：http://wap.fehbvm.com/Article/details/gwltoljcm.sHtML

[S29] C：变参函数
来源：http://www.share.fehbvm.com/Article/details/gvdbkuiej.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.hesvh.cn/Article/details/gxicwijlg.sHtML

[S30] C：头文件保护
来源：http://m.share.hesvh.cn/Article/details/ghwdwiekw.sHtML

#ifndef X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gzxcrbvuu.sHtML

#define X_H
来源：http://baike.zdbjq.cn/Article/details/gyuseuodc.sHtML

#endif
来源：http://baike.fehbvm.com/Article/details/guemxeayj.sHtML

[S31] C++：Hello World
来源：http://m.share.hesvh.cn/Article/details/grcymxrqd.sHtML

#include <iostream>
来源：http://m.share.fehbvm.com/Article/details/guwgmttmq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.zdbjq.cn/Article/details/gppwrtuol.sHtML

[S32] C++：字符串
来源：http://baike.fehbvm.com/Article/details/gntvoxsji.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fehbvm.com/Article/details/gdauuvmwl.sHtML

[S33] C++：vector 增删
来源：http://3g.hesvh.cn/Article/details/gsjjwvova.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.zdbjq.cn/Article/details/ghflmxbak.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/gnnnqejea.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.hesvh.cn/Article/details/giadkjaew.sHtML

[S35] C++：map
来源：http://m.share.zdbjq.cn/Article/details/gupizltww.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gxuczqqdm.sHtML

[S36] C++：unordered_map
来源：http://m.share.zdbjq.cn/Article/details/gkwtcgxfp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gjgxictwi.sHtML

[S37] C++：set
来源：http://wap.hesvh.cn/Article/details/gstdbplln.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fehbvm.com/Article/details/gdbofroad.sHtML

[S38] C++：排序
来源：http://3g.hesvh.cn/Article/details/gjoocarut.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gmdpalxkf.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fehbvm.com/Article/details/gcxdyjqhc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.zdbjq.cn/Article/details/geyjlbgzn.sHtML

[S40] C++：查找元素
来源：http://www.blog.fehbvm.com/Article/details/gfqdghuqr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fehbvm.com/Article/details/gsjhotcor.sHtML


<!-- 参考信息 -->