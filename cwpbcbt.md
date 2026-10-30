代发 wailian999

SHOW INDEX FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gxjzixzkv.sHtML

[Q73] 查看表状态
来源：http://www.blog.hesvh.cn/Article/details/giqkmipax.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fehbvm.com/Article/details/gpkxbqoer.sHtML

[Q74] 强制使用索引
来源：http://www.share.hesvh.cn/Article/details/grdhmtrrw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.hesvh.cn/Article/details/grbytcpnr.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gqjdbqrze.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/ggtcugcon.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.zdbjq.cn/Article/details/gtrbklfue.sHtML

[Q76] 按天统计
来源：http://www.share.zdbjq.cn/Article/details/gorqyufve.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fehbvm.com/Article/details/gymxevhst.sHtML

[Q77] 时间加减
来源：http://read.share.zdbjq.cn/Article/details/gabokujov.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.zdbjq.cn/Article/details/gucdwnwjb.sHtML

[Q78] 当前时间
来源：http://www.blog.zdbjq.cn/Article/details/gmcwqnzxg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.hesvh.cn/Article/details/gbhxxstst.sHtML

[Q79] 字符串拼接
来源：http://baike.hesvh.cn/Article/details/glsvonvgd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fehbvm.com/Article/details/gwaaxfuxq.sHtML

[Q80] 字符串截取
来源：http://www.blog.zdbjq.cn/Article/details/gfopplzsj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gwkutpfny.sHtML

[Q81] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gzistzsou.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.hesvh.cn/Article/details/glgzkzpll.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.hesvh.cn/Article/details/gotaoegmq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gacvsjrjb.sHtML

[Q83] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gfukzfwwz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gpewxxdrb.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gzcbhagfx.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gluawpale.sHtML

[Q85] 数值取整
来源：http://blog.fehbvm.com/Article/details/gpdklikhd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fehbvm.com/Article/details/gsjcmtrlt.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.hesvh.cn/Article/details/gqoitxywu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fehbvm.com/Article/details/gfmrycrxw.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.zdbjq.cn/Article/details/gmzqlqfpm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.zdbjq.cn/Article/details/gbpffxvla.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.hesvh.cn/Article/details/gyxwdjjoz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.hesvh.cn/Article/details/gldiwzvcg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.zdbjq.cn/Article/details/glvqpyzan.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.hesvh.cn/Article/details/gspqqwiim.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.hesvh.cn/Article/details/ghgplffkv.sHtML

[Q90] 生成序号列
来源：http://www.m.share.hesvh.cn/Article/details/gdkruofow.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.hesvh.cn/Article/details/gmxcekbhw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gvddrsdyf.sHtML

R. Bash 专题
来源：http://www.share.zdbjq.cn/Article/details/gmnvofpbu.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gllckpcba.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fehbvm.com/Article/details/ggvpurmec.sHtML

#!/usr/bin/env bash
来源：http://read.share.zdbjq.cn/Article/details/gpakpcmar.sHtML

set -euo pipefail
来源：http://3g.fehbvm.com/Article/details/gxqichlxf.sHtML

[R02] 变量赋值与使用
来源：http://baike.hesvh.cn/Article/details/gecdnzfrm.sHtML

name="Tom"; echo "$name"
来源：http://3g.zdbjq.cn/Article/details/gimjvglfa.sHtML

[R03] 只读变量
来源：http://blog.fehbvm.com/Article/details/ghwjuzxcr.sHtML

readonly PI=3.14
来源：http://mobile.zdbjq.cn/Article/details/gcuzaptpf.sHtML

[R04] 位置参数
来源：http://www.share.zdbjq.cn/Article/details/gwpqgyebo.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fehbvm.com/Article/details/grmqigmtf.sHtML

[R05] 参数默认值
来源：http://wap.hesvh.cn/Article/details/gwfgsppaj.sHtML

name="${1:-default}"
来源：http://mobile.fehbvm.com/Article/details/gyjzzboeh.sHtML

[R06] 判断命令是否存在
来源：http://blog.hesvh.cn/Article/details/gacgwbeew.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gxrzpeulr.sHtML

[R07] if 判断文件
来源：http://mobile.zdbjq.cn/Article/details/gqludcwga.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gnszupqrt.sHtML

[R08] 数值比较
来源：http://www.share.zdbjq.cn/Article/details/gflenfbzg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fehbvm.com/Article/details/gnzkkvlkf.sHtML

[R09] 字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gumpqqqxi.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.hesvh.cn/Article/details/gwkglbkjl.sHtML

[R10] 正则匹配
来源：http://www.share.fehbvm.com/Article/details/gsunjxnty.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.zdbjq.cn/Article/details/gffuswyku.sHtML

[R11] case 多分支
来源：http://read.share.hesvh.cn/Article/details/gyuyhjjre.sHtML

case "$1" in
来源：http://www.blog.zdbjq.cn/Article/details/gsfxdearp.sHtML

start) echo "启动" ;;
来源：http://3g.fehbvm.com/Article/details/globdslrf.sHtML

stop)  echo "停止" ;;
来源：http://baike.hesvh.cn/Article/details/gvpbtaoyo.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/gnlzwdbvi.sHtML

esac
来源：http://www.blog.hesvh.cn/Article/details/gnyskodeq.sHtML

[R12] for 遍历文件
来源：http://mobile.fehbvm.com/Article/details/gzpnmxpiw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/gyztvpbhk.sHtML

[R13] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/ggdsfacml.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gyczdefwc.sHtML

[R14] C 风格 for
来源：http://blog.hesvh.cn/Article/details/gdwkyowfc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gltoxopmn.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/glgpgeokd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fehbvm.com/Article/details/gvtafzoxg.sHtML

[R16] until 等待条件
来源：http://read.share.fehbvm.com/Article/details/gzvttjhvo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gaaqyyozc.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/gplzjvqtv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fehbvm.com/Article/details/gnnnxyrks.sHtML

[R18] 遍历数组
来源：http://blog.hesvh.cn/Article/details/guojzpxqq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.zdbjq.cn/Article/details/guscgvnaf.sHtML

[R19] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gjdxhabtt.sHtML

echo "${#arr[@]}"
来源：http://www.blog.zdbjq.cn/Article/details/gwzkqsmdw.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fehbvm.com/Article/details/gywcrqant.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.hesvh.cn/Article/details/ggadrlcfm.sHtML

[R21] 字符串长度
来源：http://blog.hesvh.cn/Article/details/glulywsgn.sHtML

echo "${#s}"
来源：http://www.share.zdbjq.cn/Article/details/gyrutadnj.sHtML

[R22] 截取子串
来源：http://m.share.hesvh.cn/Article/details/gkmbwhnko.sHtML

echo "${s:0:5}"
来源：http://read.share.zdbjq.cn/Article/details/giouhtcbl.sHtML

[R23] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gjorpajvg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fehbvm.com/Article/details/griubmmfj.sHtML

[R24] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gujjmcglo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fehbvm.com/Article/details/gnoqxhjib.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.hesvh.cn/Article/details/glbvmjprs.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fehbvm.com/Article/details/gcscvgqmh.sHtML

[R26] 命令替换
来源：http://www.blog.hesvh.cn/Article/details/gfuplqgkm.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fehbvm.com/Article/details/gyaupghoj.sHtML

[R27] 算术展开
来源：http://www.blog.hesvh.cn/Article/details/gaxxcpxdw.sHtML

echo $((1 + 2 * 3))
来源：http://baike.hesvh.cn/Article/details/gsfevsgmq.sHtML

[R28] 浮点运算
来源：http://blog.fehbvm.com/Article/details/gllhzkesn.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fehbvm.com/Article/details/gjhazxkbi.sHtML

[R29] 定义函数
来源：http://www.share.fehbvm.com/Article/details/glatslypo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fehbvm.com/Article/details/gbobcwdzf.sHtML

[R30] 函数返回状态码
来源：http://baike.hesvh.cn/Article/details/gpadohihi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.hesvh.cn/Article/details/gvhwjgmnc.sHtML

[R31] 局部变量
来源：http://www.blog.hesvh.cn/Article/details/gxmuxpjvm.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.zdbjq.cn/Article/details/ghtghdxwh.sHtML

[R32] 参数个数校验
来源：http://wap.hesvh.cn/Article/details/gcvlaoqyn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gewynikih.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.hesvh.cn/Article/details/gjddtbrih.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fehbvm.com/Article/details/gufybdefp.sHtML

[R34] 退出时清理
来源：http://read.share.hesvh.cn/Article/details/gekidkdnl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gtzasxnvz.sHtML

[R35] 后台执行并等待
来源：http://3g.hesvh.cn/Article/details/gehogzjmu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.zdbjq.cn/Article/details/gqgidzaqd.sHtML

[R36] 并发执行多个任务
来源：http://blog.fehbvm.com/Article/details/gfrfxvcpe.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fehbvm.com/Article/details/gvzzpdrnn.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.hesvh.cn/Article/details/givymkrtz.sHtML

files=$(ls -1)
来源：http://wap.zdbjq.cn/Article/details/gmxossyeg.sHtML

[R38] 管道串联
来源：http://m.share.zdbjq.cn/Article/details/ggfvjilft.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.hesvh.cn/Article/details/goantodtz.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.hesvh.cn/Article/details/ghkqutape.sHtML

cmd > out.log 2>&1
来源：http://m.share.zdbjq.cn/Article/details/guudoubye.sHtML

[R40] 追加写日志
来源：http://read.share.fehbvm.com/Article/details/gcureoucy.sHtML

echo "log" >> out.log
来源：http://www.blog.hesvh.cn/Article/details/grtjwjkoa.sHtML

[R41] 丢弃输出
来源：http://m.share.zdbjq.cn/Article/details/gamvifbxx.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fehbvm.com/Article/details/ghuajzabk.sHtML

[R42] 输入重定向
来源：http://wap.fehbvm.com/Article/details/gvwgigspi.sHtML

wc -l < a.txt
来源：http://m.share.zdbjq.cn/Article/details/gdmcvhnhc.sHtML

[R43] 按名字查找文件
来源：http://3g.hesvh.cn/Article/details/guofedlsr.sHtML

find . -name "*.log" -type f
来源：http://wap.fehbvm.com/Article/details/gluncgcyz.sHtML

[R44] 按修改时间查找
来源：http://blog.fehbvm.com/Article/details/goxxpddcf.sHtML

find . -mtime -7 -type f
来源：http://mobile.zdbjq.cn/Article/details/gjwthfpnb.sHtML

[R45] 批量删除
来源：http://baike.fehbvm.com/Article/details/gxfygbktr.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fehbvm.com/Article/details/gnjmnvvyn.sHtML

[R46] 递归替换文件内容
来源：http://3g.hesvh.cn/Article/details/gcazuaaty.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.hesvh.cn/Article/details/goqdgcqma.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/gfhuoczwi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/gyahfjmss.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/gramxetfc.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gddmuyrjd.sHtML

[R49] awk 带条件
来源：http://mobile.hesvh.cn/Article/details/gcnfdiifm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fehbvm.com/Article/details/goebrzgbm.sHtML

[R50] awk 求和
来源：http://m.share.hesvh.cn/Article/details/gwqeymedf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gxpoihvac.sHtML

[R51] 排序去重取前几
来源：http://m.share.zdbjq.cn/Article/details/gxvatrlgn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.zdbjq.cn/Article/details/gynaclybc.sHtML

[R52] 统计行数
来源：http://blog.fehbvm.com/Article/details/gunvzmigz.sHtML

wc -l a.txt
来源：http://www.share.hesvh.cn/Article/details/gvypotzlp.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.zdbjq.cn/Article/details/gsqifzcwt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fehbvm.com/Article/details/gkxluszig.sHtML

[R54] 比较两个文件
来源：http://baike.hesvh.cn/Article/details/gsgoywxow.sHtML

diff a.txt b.txt
来源：http://blog.hesvh.cn/Article/details/gfltysdgo.sHtML

[R55] 压缩与解压
来源：http://3g.fehbvm.com/Article/details/ggfsbjiit.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/gusxhlqek.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/ggrfcnvyh.sHtML

scp file user@host:/path/
来源：http://wap.zdbjq.cn/Article/details/gfrnialkq.sHtML

[R57] 远程执行命令
来源：http://m.share.fehbvm.com/Article/details/gmokiiyhz.sHtML

ssh user@host 'uptime'
来源：http://wap.hesvh.cn/Article/details/gejvdqnuh.sHtML

[R58] 下载文件
来源：http://mobile.zdbjq.cn/Article/details/gtqkmexad.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/gjnjosdxq.sHtML

[R59] 发 POST JSON
来源：http://blog.zdbjq.cn/Article/details/glodpkrjt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.hesvh.cn/Article/details/giypaqikw.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gryfaeqzk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.zdbjq.cn/Article/details/gyorbijva.sHtML

[R61] 磁盘占用
来源：http://mobile.fehbvm.com/Article/details/grhsjieiq.sHtML

df -h;  du -sh *
来源：http://3g.fehbvm.com/Article/details/gitohkank.sHtML

[R62] 找最占空间的文件
来源：http://baike.fehbvm.com/Article/details/gutrtvlje.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.zdbjq.cn/Article/details/geqechpos.sHtML

[R63] 内存与进程
来源：http://baike.zdbjq.cn/Article/details/gjzzhjuvn.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.zdbjq.cn/Article/details/gquudscsw.sHtML

[R64] 结束进程
来源：http://blog.hesvh.cn/Article/details/gplpirrbs.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.zdbjq.cn/Article/details/gtrtbtsyq.sHtML

[R65] 查看端口占用
来源：http://read.share.zdbjq.cn/Article/details/gfkpgygbf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fehbvm.com/Article/details/guvapphaf.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/gsyzwhtrv.sHtML

crontab -e;  crontab -l
来源：http://wap.fehbvm.com/Article/details/giknauesf.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fehbvm.com/Article/details/gkmojqwxz.sHtML

openssl rand -hex 16
来源：http://www.m.share.zdbjq.cn/Article/details/gnipbfgmo.sHtML

[R68] 计算文件校验值
来源：http://blog.zdbjq.cn/Article/details/gxiktsgmu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.hesvh.cn/Article/details/gkiyhqsya.sHtML

[R69] 生成随机密码
来源：http://wap.fehbvm.com/Article/details/gbfkirqya.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.zdbjq.cn/Article/details/gerkdpfem.sHtML

[R70] 时间戳与互转
来源：http://www.share.hesvh.cn/Article/details/gdcqdbshq.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.hesvh.cn/Article/details/gkvflpclk.sHtML

[R71] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/goioulcac.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fehbvm.com/Article/details/gfwdllroq.sHtML

[R72] 等待端口就绪
来源：http://3g.zdbjq.cn/Article/details/gvnywepyx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gaojtiyfl.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/gfkotkfcl.sHtML

split -l 1000 big.log part_
来源：http://www.share.zdbjq.cn/Article/details/gqwgrmuvh.sHtML

[R74] 批量重命名
来源：http://baike.hesvh.cn/Article/details/gcinrwyuy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fehbvm.com/Article/details/gqxbwvbis.sHtML

[R75] 导出环境变量
来源：http://www.share.hesvh.cn/Article/details/ggznrejov.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/gudbznrbo.sHtML

[R76] 使用临时文件
来源：http://www.blog.fehbvm.com/Article/details/giarnboxc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gxsfrlodw.sHtML

[R77] 读取用户输入
来源：http://m.share.zdbjq.cn/Article/details/gejwwpyan.sHtML

read -rp "请输入: " ans
来源：http://wap.hesvh.cn/Article/details/gameugpqw.sHtML

[R78] 交互式菜单
来源：http://www.blog.hesvh.cn/Article/details/ggsoqzlfr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.hesvh.cn/Article/details/gngqxcvzx.sHtML

[R79] 解析命令行选项
来源：http://3g.fehbvm.com/Article/details/gwvlxraia.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.hesvh.cn/Article/details/gzdbwiqkm.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.hesvh.cn/Article/details/gigfbqcfy.sHtML

time ./run.sh
来源：http://3g.zdbjq.cn/Article/details/gdojsynlf.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gnngzyvqu.sHtML

S. C / C++ 专题
来源：http://read.share.zdbjq.cn/Article/details/glmcwjawh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gfnjfxqpg.sHtML

[S01] C：Hello World
来源：http://www.share.hesvh.cn/Article/details/gupktblgh.sHtML

#include <stdio.h>
来源：http://read.share.fehbvm.com/Article/details/gmorgzjma.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.zdbjq.cn/Article/details/gpmoswogt.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gljnjswxf.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.zdbjq.cn/Article/details/gvstjxavm.sHtML

[S03] C：读入整数
来源：http://www.m.share.hesvh.cn/Article/details/gezpodntf.sHtML

int x; scanf("%d", &x);
来源：http://3g.zdbjq.cn/Article/details/gbzptciid.sHtML

[S04] C：字符串复制
来源：http://wap.fehbvm.com/Article/details/gxzgwznvk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fehbvm.com/Article/details/gnyirbhmq.sHtML

[S05] C：字符串长度
来源：http://baike.fehbvm.com/Article/details/gbzadjgxx.sHtML

strlen(s)
来源：http://blog.hesvh.cn/Article/details/gefdnyreh.sHtML

[S06] C：字符串比较
来源：http://read.share.hesvh.cn/Article/details/gusvlpior.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.hesvh.cn/Article/details/gpnbzejqi.sHtML

[S07] C：数组遍历求和
来源：http://m.share.zdbjq.cn/Article/details/gceszcxpk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.hesvh.cn/Article/details/gnunczzgy.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.hesvh.cn/Article/details/gnahplxzk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fehbvm.com/Article/details/guunhshmg.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.hesvh.cn/Article/details/gkrzhqvij.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/golirnulj.sHtML

[S10] C：指针与解引用
来源：http://baike.zdbjq.cn/Article/details/gxcvzysyb.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gfjzjlgrv.sHtML

[S11] C：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gzvmcrohf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.hesvh.cn/Article/details/gvozfcwjg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/gkjibhlzd.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gigiiuigb.sHtML

[S12] C：写文件
来源：http://wap.fehbvm.com/Article/details/ggtptdzvm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fehbvm.com/Article/details/ggwajgays.sHtML

[S13] C：宏定义
来源：http://m.share.fehbvm.com/Article/details/glvpytwul.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/gowqazsqp.sHtML

[S14] C：枚举
来源：http://baike.fehbvm.com/Article/details/ggymfmtil.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.zdbjq.cn/Article/details/gfyegsubi.sHtML

[S15] C：类型转换
来源：http://mobile.fehbvm.com/Article/details/gjklcfvnz.sHtML

(double) a / b
来源：http://3g.fehbvm.com/Article/details/gggztwjed.sHtML

[S16] C：位操作置位
来源：http://blog.hesvh.cn/Article/details/gqddasmdd.sHtML

x |= (1 << 3);
来源：http://m.share.hesvh.cn/Article/details/gjsaefkxa.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/goxgwcjeh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.hesvh.cn/Article/details/gvicqyfja.sHtML

[S18] C：命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gdmadbmin.sHtML

int main(int argc, char **argv)
来源：http://wap.fehbvm.com/Article/details/gvlmvqlrv.sHtML

[S19] C：快速排序
来源：http://www.blog.zdbjq.cn/Article/details/gzaoviocz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gfrsidwbm.sHtML

[S20] C：二分查找
来源：http://www.share.hesvh.cn/Article/details/gunkiyqzw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gxxapojgt.sHtML

[S21] C：字符类别判断
来源：http://www.share.zdbjq.cn/Article/details/gwifamlrs.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fehbvm.com/Article/details/gbipslnwx.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/gjfqpyiri.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.zdbjq.cn/Article/details/gdxdjbpdu.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/guldddwaq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fehbvm.com/Article/details/gxvdkiuyg.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fehbvm.com/Article/details/gqzslmwic.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fehbvm.com/Article/details/ghgindshh.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/ghkwklkde.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/glwcyrxlp.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/gyeqcmvze.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/gefknujaq.sHtML

[S27] C：定义常量
来源：http://www.m.share.zdbjq.cn/Article/details/gbzmupllk.sHtML

const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gunifiaal.sHtML

[S28] C：静态变量
来源：http://3g.zdbjq.cn/Article/details/gorcphqdq.sHtML

static int counter = 0;
来源：http://www.share.fehbvm.com/Article/details/gbwqjfxho.sHtML

[S29] C：变参函数
来源：http://baike.zdbjq.cn/Article/details/gcxksttxs.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.zdbjq.cn/Article/details/gcrxolero.sHtML

[S30] C：头文件保护
来源：http://m.share.fehbvm.com/Article/details/glenjvlpy.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/gfquqpzrv.sHtML

#define X_H
来源：http://www.m.share.zdbjq.cn/Article/details/ggssjwfaq.sHtML

#endif
来源：http://www.blog.hesvh.cn/Article/details/gactydhzt.sHtML

[S31] C++：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gmgscqoxu.sHtML

#include <iostream>
来源：http://wap.hesvh.cn/Article/details/gbyeqzvmz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fehbvm.com/Article/details/gihdlbfgd.sHtML

[S32] C++：字符串
来源：http://3g.zdbjq.cn/Article/details/gavqqtkzk.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fehbvm.com/Article/details/glddokjkj.sHtML

[S33] C++：vector 增删
来源：http://baike.hesvh.cn/Article/details/gkaagnunu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.zdbjq.cn/Article/details/gsgbnltsb.sHtML

[S34] C++：遍历 vector
来源：http://www.share.hesvh.cn/Article/details/grmbeoofa.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fehbvm.com/Article/details/gwozyoyya.sHtML

[S35] C++：map
来源：http://www.blog.zdbjq.cn/Article/details/gfrdysgsi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gghscwgxi.sHtML

[S36] C++：unordered_map
来源：http://read.share.zdbjq.cn/Article/details/gixprrwqp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gumsiktpe.sHtML

[S37] C++：set
来源：http://www.blog.zdbjq.cn/Article/details/gqqgmuohm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.hesvh.cn/Article/details/guvqpoxdu.sHtML

[S38] C++：排序
来源：http://baike.zdbjq.cn/Article/details/gydowabxd.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.hesvh.cn/Article/details/gavuayzrg.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/gsuzlsahg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fehbvm.com/Article/details/ghefvlyow.sHtML

[S40] C++：查找元素
来源：http://3g.fehbvm.com/Article/details/gufwdptjk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.zdbjq.cn/Article/details/gecbckzeg.sHtML

[S41] C++：类与构造函数
来源：http://www.share.hesvh.cn/Article/details/gtfjqgrza.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fehbvm.com/Article/details/gsgycgbor.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.zdbjq.cn/Article/details/gyooqkuei.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/gvfmmwlxv.sHtML


<!-- 参考信息 -->