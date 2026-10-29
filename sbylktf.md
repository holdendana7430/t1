代发 wailian999

[Q76] 按天统计
来源：http://m.share.hesvh.cn/Article/details/gvwjxjmuu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fehbvm.com/Article/details/gdlzasqsp.sHtML

[Q77] 时间加减
来源：http://wap.hesvh.cn/Article/details/gbvopdpko.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.zdbjq.cn/Article/details/gbffrtzva.sHtML

[Q78] 当前时间
来源：http://www.m.share.zdbjq.cn/Article/details/gksljomov.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.zdbjq.cn/Article/details/gvjfgxfvv.sHtML

[Q79] 字符串拼接
来源：http://wap.fehbvm.com/Article/details/gswocckzj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.zdbjq.cn/Article/details/gqucpirvt.sHtML

[Q80] 字符串截取
来源：http://www.blog.fehbvm.com/Article/details/gcszurawd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gddganxts.sHtML

[Q81] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gplvwjzum.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.zdbjq.cn/Article/details/ghqgtjfxr.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fehbvm.com/Article/details/gxyuzxpan.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gbwymrvqo.sHtML

[Q83] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gcdctecpy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gohvwejxv.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gfgyhdtxi.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gdblvfjdy.sHtML

[Q85] 数值取整
来源：http://m.share.fehbvm.com/Article/details/gefeprgge.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fehbvm.com/Article/details/gsuuisnca.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.hesvh.cn/Article/details/gdgkgtcru.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fehbvm.com/Article/details/gatboipva.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fehbvm.com/Article/details/gxdjlptru.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fehbvm.com/Article/details/gunuyvszb.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fehbvm.com/Article/details/gsnwqowmb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.zdbjq.cn/Article/details/gcjcbrara.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.hesvh.cn/Article/details/gkiokyvss.sHtML

[Q89] 判断表是否存在
来源：http://read.share.hesvh.cn/Article/details/gyxcekfox.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.hesvh.cn/Article/details/gnglbiuil.sHtML

[Q90] 生成序号列
来源：http://www.m.share.hesvh.cn/Article/details/gkpvmcrtf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.hesvh.cn/Article/details/gxxtxvvac.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gepzaeyur.sHtML

R. Bash 专题
来源：http://wap.zdbjq.cn/Article/details/gssllerav.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqsstlsqd.sHtML

[R01] shebang 与严格模式
来源：http://www.share.zdbjq.cn/Article/details/gnmkraxzg.sHtML

#!/usr/bin/env bash
来源：http://wap.zdbjq.cn/Article/details/gzpgfrkcj.sHtML

set -euo pipefail
来源：http://www.m.share.zdbjq.cn/Article/details/gggckbuxg.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fehbvm.com/Article/details/gbmutvjdj.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fehbvm.com/Article/details/gdlldtwhk.sHtML

[R03] 只读变量
来源：http://m.share.zdbjq.cn/Article/details/glnqvssgq.sHtML

readonly PI=3.14
来源：http://baike.fehbvm.com/Article/details/gfffnkzqy.sHtML

[R04] 位置参数
来源：http://blog.hesvh.cn/Article/details/ggsyameef.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.hesvh.cn/Article/details/gsivuzuwa.sHtML

[R05] 参数默认值
来源：http://read.share.zdbjq.cn/Article/details/ghaxwuwus.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/gpgotfajy.sHtML

[R06] 判断命令是否存在
来源：http://mobile.zdbjq.cn/Article/details/gdknmsype.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gjqlsrliz.sHtML

[R07] if 判断文件
来源：http://wap.hesvh.cn/Article/details/gwcrqjftg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.zdbjq.cn/Article/details/gbrwkzgdo.sHtML

[R08] 数值比较
来源：http://www.m.share.hesvh.cn/Article/details/gsvxnyvnr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.zdbjq.cn/Article/details/grjkkwskb.sHtML

[R09] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/ggaygkvgq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.zdbjq.cn/Article/details/gjcohqowj.sHtML

[R10] 正则匹配
来源：http://3g.zdbjq.cn/Article/details/gpvuvtrap.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.hesvh.cn/Article/details/gkdofqlxb.sHtML

[R11] case 多分支
来源：http://mobile.hesvh.cn/Article/details/gyuvtazuy.sHtML

case "$1" in
来源：http://m.share.fehbvm.com/Article/details/gjlmliwej.sHtML

start) echo "启动" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/guexmwmxm.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gbxkupnpb.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.hesvh.cn/Article/details/glawwllct.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/gjhtgaxge.sHtML

[R12] for 遍历文件
来源：http://3g.fehbvm.com/Article/details/gboipxqkb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fehbvm.com/Article/details/gjkudxioi.sHtML

[R13] for 计数循环
来源：http://www.blog.hesvh.cn/Article/details/gavybdzxp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/grutfzlxe.sHtML

[R14] C 风格 for
来源：http://www.m.share.zdbjq.cn/Article/details/gykicvexh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gudfycpvb.sHtML

[R15] while 逐行读文件
来源：http://3g.zdbjq.cn/Article/details/glvvvedak.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.hesvh.cn/Article/details/gbqjgetkz.sHtML

[R16] until 等待条件
来源：http://www.share.fehbvm.com/Article/details/gnpjzfbib.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/glwywioqx.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/gmpevizjc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.hesvh.cn/Article/details/gdhadsioe.sHtML

[R18] 遍历数组
来源：http://wap.zdbjq.cn/Article/details/gzqbvsuvn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.zdbjq.cn/Article/details/ggmbqqjxw.sHtML

[R19] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gqjrpmjoz.sHtML

echo "${#arr[@]}"
来源：http://baike.fehbvm.com/Article/details/gmjrzyylm.sHtML

[R20] 关联数组（字典）
来源：http://blog.hesvh.cn/Article/details/gtshaophr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/gjcespeen.sHtML

[R21] 字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gjxedwqki.sHtML

echo "${#s}"
来源：http://m.share.fehbvm.com/Article/details/gbkulomko.sHtML

[R22] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gwkjjkjef.sHtML

echo "${s:0:5}"
来源：http://wap.hesvh.cn/Article/details/gtqimktle.sHtML

[R23] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gjwfcrlvj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.hesvh.cn/Article/details/gopmhcpji.sHtML

[R24] 大小写转换
来源：http://baike.hesvh.cn/Article/details/ghaxmszwi.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fehbvm.com/Article/details/gllqkvshu.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.hesvh.cn/Article/details/gexudlifk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.zdbjq.cn/Article/details/gawdsumwu.sHtML

[R26] 命令替换
来源：http://m.share.fehbvm.com/Article/details/gfwqctfdn.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/ghplfffjn.sHtML

[R27] 算术展开
来源：http://m.share.fehbvm.com/Article/details/gmakvyomx.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fehbvm.com/Article/details/gxjeiwsfo.sHtML

[R28] 浮点运算
来源：http://www.m.share.zdbjq.cn/Article/details/gggoiwatq.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.hesvh.cn/Article/details/gbnvcimdx.sHtML

[R29] 定义函数
来源：http://mobile.fehbvm.com/Article/details/gnnfocphy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fehbvm.com/Article/details/giyjxepxf.sHtML

[R30] 函数返回状态码
来源：http://baike.hesvh.cn/Article/details/gpexfjihr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.zdbjq.cn/Article/details/gmzetsocd.sHtML

[R31] 局部变量
来源：http://www.share.fehbvm.com/Article/details/glgcftmng.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.zdbjq.cn/Article/details/gdxaipdve.sHtML

[R32] 参数个数校验
来源：http://www.share.fehbvm.com/Article/details/geutoxqkq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gtbdvspht.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.hesvh.cn/Article/details/gytgrkyub.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fehbvm.com/Article/details/grzepyneu.sHtML

[R34] 退出时清理
来源：http://wap.fehbvm.com/Article/details/gamxluwtb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gqbwqqzfc.sHtML

[R35] 后台执行并等待
来源：http://www.share.hesvh.cn/Article/details/golmzzlux.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.hesvh.cn/Article/details/gteghxezt.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fehbvm.com/Article/details/gxzepsqwx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/gibhhbbkq.sHtML

[R37] 把输出赋给变量
来源：http://www.share.zdbjq.cn/Article/details/gzqtlylvc.sHtML

files=$(ls -1)
来源：http://www.share.zdbjq.cn/Article/details/gcazrjxgy.sHtML

[R38] 管道串联
来源：http://wap.hesvh.cn/Article/details/ggnidoedz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fehbvm.com/Article/details/gqhbpdcaw.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.zdbjq.cn/Article/details/gvfuwcvne.sHtML

cmd > out.log 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gtrgozxhu.sHtML

[R40] 追加写日志
来源：http://blog.zdbjq.cn/Article/details/ggiimauom.sHtML

echo "log" >> out.log
来源：http://wap.fehbvm.com/Article/details/gcujjmvmh.sHtML

[R41] 丢弃输出
来源：http://read.share.fehbvm.com/Article/details/giydrvozt.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fehbvm.com/Article/details/geecaetuu.sHtML

[R42] 输入重定向
来源：http://www.m.share.zdbjq.cn/Article/details/gtdkdzslb.sHtML

wc -l < a.txt
来源：http://m.share.hesvh.cn/Article/details/ghiaqzybu.sHtML

[R43] 按名字查找文件
来源：http://blog.fehbvm.com/Article/details/gqgqpdyfa.sHtML

find . -name "*.log" -type f
来源：http://wap.hesvh.cn/Article/details/ghrperygb.sHtML

[R44] 按修改时间查找
来源：http://blog.fehbvm.com/Article/details/giweutwne.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.hesvh.cn/Article/details/gswwerhtl.sHtML

[R45] 批量删除
来源：http://wap.zdbjq.cn/Article/details/guhfxyxwv.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fehbvm.com/Article/details/gjfxhabav.sHtML

[R46] 递归替换文件内容
来源：http://3g.hesvh.cn/Article/details/gfhqyvnls.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fehbvm.com/Article/details/guqpaocmm.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fehbvm.com/Article/details/gssmhrxlw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gucgqrwgf.sHtML

[R48] awk 取指定列
来源：http://mobile.hesvh.cn/Article/details/gyirvkrna.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gdzqvnndl.sHtML

[R49] awk 带条件
来源：http://m.share.fehbvm.com/Article/details/gsjleayqy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fehbvm.com/Article/details/godcbiwcw.sHtML

[R50] awk 求和
来源：http://www.share.fehbvm.com/Article/details/gsxhmpccu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gncmhboqq.sHtML

[R51] 排序去重取前几
来源：http://wap.zdbjq.cn/Article/details/gvswzmegy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.zdbjq.cn/Article/details/gubdktkdg.sHtML

[R52] 统计行数
来源：http://m.share.fehbvm.com/Article/details/gozkgluzl.sHtML

wc -l a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gafnycxge.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fehbvm.com/Article/details/ggporqnxi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.zdbjq.cn/Article/details/gxdfhedgd.sHtML

[R54] 比较两个文件
来源：http://3g.hesvh.cn/Article/details/geapmiloc.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gbdbbewpp.sHtML

[R55] 压缩与解压
来源：http://3g.hesvh.cn/Article/details/giydhjrkx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.hesvh.cn/Article/details/gbymluppr.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/gaznbyfup.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/gpxexcrlh.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/gxburrdnm.sHtML

ssh user@host 'uptime'
来源：http://www.share.zdbjq.cn/Article/details/gfnutijcd.sHtML

[R58] 下载文件
来源：http://baike.fehbvm.com/Article/details/galpuhits.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fehbvm.com/Article/details/gkclulzpd.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gxzoaoxzi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.hesvh.cn/Article/details/geylrkdut.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/geruwspye.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fehbvm.com/Article/details/gdnwaqpac.sHtML

[R61] 磁盘占用
来源：http://mobile.fehbvm.com/Article/details/giaeophim.sHtML

df -h;  du -sh *
来源：http://wap.fehbvm.com/Article/details/grcnrrwke.sHtML

[R62] 找最占空间的文件
来源：http://read.share.hesvh.cn/Article/details/ghpbvwhib.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/gykiubwqf.sHtML

[R63] 内存与进程
来源：http://read.share.zdbjq.cn/Article/details/ggcijgubs.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.hesvh.cn/Article/details/gyltzygzd.sHtML

[R64] 结束进程
来源：http://mobile.zdbjq.cn/Article/details/gdhbgcxid.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fehbvm.com/Article/details/ghefamkzo.sHtML

[R65] 查看端口占用
来源：http://3g.zdbjq.cn/Article/details/gmcehnjyq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.zdbjq.cn/Article/details/ggirygvji.sHtML

[R66] 定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gxsmsrlyf.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fehbvm.com/Article/details/gdkzwuxuy.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fehbvm.com/Article/details/gkatdtupc.sHtML

openssl rand -hex 16
来源：http://baike.hesvh.cn/Article/details/gqjzqeejb.sHtML

[R68] 计算文件校验值
来源：http://wap.zdbjq.cn/Article/details/ghvwtqnei.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.hesvh.cn/Article/details/ghzxtfsmt.sHtML

[R69] 生成随机密码
来源：http://read.share.fehbvm.com/Article/details/gpcapinai.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.zdbjq.cn/Article/details/gqncasshq.sHtML

[R70] 时间戳与互转
来源：http://www.share.fehbvm.com/Article/details/gmkwgqool.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.zdbjq.cn/Article/details/gopihdoga.sHtML

[R71] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gdcjrqyck.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.zdbjq.cn/Article/details/gmlxyzeqj.sHtML

[R72] 等待端口就绪
来源：http://baike.zdbjq.cn/Article/details/gjhnbpbzf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gdihfbexk.sHtML

[R73] 分割大日志
来源：http://baike.zdbjq.cn/Article/details/gddwyplwm.sHtML

split -l 1000 big.log part_
来源：http://m.share.hesvh.cn/Article/details/gwcsefuvu.sHtML

[R74] 批量重命名
来源：http://www.m.share.fehbvm.com/Article/details/ghchcbgym.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.zdbjq.cn/Article/details/ghojfkfvb.sHtML

[R75] 导出环境变量
来源：http://blog.fehbvm.com/Article/details/guqvazfzu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.hesvh.cn/Article/details/giunfbamo.sHtML

[R76] 使用临时文件
来源：http://baike.hesvh.cn/Article/details/ggelskhrb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gkuihdeei.sHtML

[R77] 读取用户输入
来源：http://m.share.hesvh.cn/Article/details/gwfbedfyy.sHtML

read -rp "请输入: " ans
来源：http://3g.zdbjq.cn/Article/details/gsyfkfgpu.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/gmueghcsg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.zdbjq.cn/Article/details/gpxeyzhaw.sHtML

[R79] 解析命令行选项
来源：http://blog.hesvh.cn/Article/details/gcoasqfzm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fehbvm.com/Article/details/glhdhptvm.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.hesvh.cn/Article/details/gyixolepf.sHtML

time ./run.sh
来源：http://www.blog.zdbjq.cn/Article/details/gctxuitgc.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmdquyexu.sHtML

S. C / C++ 专题
来源：http://read.share.hesvh.cn/Article/details/gbmizlrss.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gopghjuzr.sHtML

[S01] C：Hello World
来源：http://read.share.hesvh.cn/Article/details/gznhowypk.sHtML

#include <stdio.h>
来源：http://m.share.fehbvm.com/Article/details/gbhoyjvxc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fehbvm.com/Article/details/goqtcgovr.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fehbvm.com/Article/details/gjubzxgzr.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.zdbjq.cn/Article/details/gndzcuqna.sHtML

[S03] C：读入整数
来源：http://3g.hesvh.cn/Article/details/gznjrrvds.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fehbvm.com/Article/details/gzkdxyzeo.sHtML

[S04] C：字符串复制
来源：http://www.share.zdbjq.cn/Article/details/ggchmxsky.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gnfsblzry.sHtML

[S05] C：字符串长度
来源：http://baike.fehbvm.com/Article/details/gqvvniizd.sHtML

strlen(s)
来源：http://baike.fehbvm.com/Article/details/gxvzfnwgw.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/gsjrlzvic.sHtML

strcmp(a, b) == 0
来源：http://blog.fehbvm.com/Article/details/gvyqmmxna.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.hesvh.cn/Article/details/ggtrdsrat.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fehbvm.com/Article/details/gagtxqnzt.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.zdbjq.cn/Article/details/gqnyxzowg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.zdbjq.cn/Article/details/gsgpjkcoc.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fehbvm.com/Article/details/gpzdahcdy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.zdbjq.cn/Article/details/gjgykzsyi.sHtML

[S10] C：指针与解引用
来源：http://3g.hesvh.cn/Article/details/gjlxwcpcf.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/gqrbhrucg.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gxfhnouxm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/gdtclrhdj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.hesvh.cn/Article/details/givyckekd.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gvfpntwut.sHtML

[S12] C：写文件
来源：http://3g.zdbjq.cn/Article/details/giwwqsmyl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gukjrubig.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/gcsrsnoue.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fehbvm.com/Article/details/gfpoqkxsl.sHtML

[S14] C：枚举
来源：http://mobile.zdbjq.cn/Article/details/gazorjrdc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fehbvm.com/Article/details/gynnsymes.sHtML

[S15] C：类型转换
来源：http://3g.zdbjq.cn/Article/details/gcsxaigrd.sHtML

(double) a / b
来源：http://www.share.fehbvm.com/Article/details/gmjtgxpfc.sHtML

[S16] C：位操作置位
来源：http://blog.fehbvm.com/Article/details/gdtlwltkw.sHtML

x |= (1 << 3);
来源：http://www.blog.hesvh.cn/Article/details/gnzjruutb.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gnhggwgrl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.hesvh.cn/Article/details/gjjappibk.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gxzttwkjh.sHtML

int main(int argc, char **argv)
来源：http://www.blog.hesvh.cn/Article/details/ggvqrqevw.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/gahwrewym.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gczexkptf.sHtML

[S20] C：二分查找
来源：http://www.m.share.hesvh.cn/Article/details/gglqbnjeb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gklynlqxk.sHtML

[S21] C：字符类别判断
来源：http://wap.hesvh.cn/Article/details/gpkoymvrj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.zdbjq.cn/Article/details/gxvrfmokp.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/gyjzhrsez.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/gitopnyoe.sHtML

[S23] C：随机数
来源：http://wap.fehbvm.com/Article/details/gifpwudor.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fehbvm.com/Article/details/gpxxbuoob.sHtML

[S24] C：获取本地时间
来源：http://baike.zdbjq.cn/Article/details/ghhvtigqv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fehbvm.com/Article/details/gccclxkgd.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/gyhfkifux.sHtML

memcpy(dst, src, n);
来源：http://m.share.zdbjq.cn/Article/details/gxsvhtqgb.sHtML

[S26] C：内存清零
来源：http://www.blog.zdbjq.cn/Article/details/gwdxphfoj.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fehbvm.com/Article/details/gojemydqc.sHtML

[S27] C：定义常量
来源：http://baike.hesvh.cn/Article/details/gearjybov.sHtML

const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gdlageepj.sHtML

[S28] C：静态变量
来源：http://mobile.fehbvm.com/Article/details/gebcswqbe.sHtML

static int counter = 0;
来源：http://www.share.zdbjq.cn/Article/details/gsqchiieo.sHtML

[S29] C：变参函数
来源：http://m.share.fehbvm.com/Article/details/gwepfghxa.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.hesvh.cn/Article/details/glfjaumcc.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/gkglwrdxy.sHtML

#ifndef X_H
来源：http://read.share.zdbjq.cn/Article/details/gywdqxsts.sHtML

#define X_H
来源：http://blog.fehbvm.com/Article/details/gndxxqiib.sHtML

#endif
来源：http://wap.fehbvm.com/Article/details/gymstgihr.sHtML

[S31] C++：Hello World
来源：http://baike.hesvh.cn/Article/details/gedoakrnx.sHtML

#include <iostream>
来源：http://m.share.fehbvm.com/Article/details/gdjkwnbxb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.hesvh.cn/Article/details/gzxmnnell.sHtML

[S32] C++：字符串
来源：http://www.blog.zdbjq.cn/Article/details/gwfihxzjf.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fehbvm.com/Article/details/gepvqrsmc.sHtML

[S33] C++：vector 增删
来源：http://blog.fehbvm.com/Article/details/gtczvotyl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.hesvh.cn/Article/details/gzsizvafl.sHtML

[S34] C++：遍历 vector
来源：http://www.share.zdbjq.cn/Article/details/gticbpubi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.hesvh.cn/Article/details/gywxhpxuz.sHtML

[S35] C++：map
来源：http://3g.hesvh.cn/Article/details/gbrdelvmh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gsfzxityo.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fehbvm.com/Article/details/gtyndhkvj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gvwcolwdj.sHtML

[S37] C++：set
来源：http://wap.zdbjq.cn/Article/details/gdlespnul.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.zdbjq.cn/Article/details/gxlvafepu.sHtML

[S38] C++：排序
来源：http://m.share.hesvh.cn/Article/details/gnxnsivvm.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gldsueiuj.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fehbvm.com/Article/details/gcnovxanb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.zdbjq.cn/Article/details/gxcpmngaz.sHtML

[S40] C++：查找元素
来源：http://mobile.hesvh.cn/Article/details/gkguvsusb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.zdbjq.cn/Article/details/gqtbiwqte.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/gzmgcelhk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fehbvm.com/Article/details/gotxqszgz.sHtML

[S42] C++：继承与虚函数
来源：http://3g.hesvh.cn/Article/details/gfeuqigxs.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fehbvm.com/Article/details/giencaqhj.sHtML

[S43] C++：智能指针
来源：http://3g.hesvh.cn/Article/details/gwtndjxdn.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/gewepoezg.sHtML

[S44] C++：引用传参
来源：http://www.share.fehbvm.com/Article/details/gaejidlfv.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.hesvh.cn/Article/details/gdayyeyqh.sHtML

[S45] C++：lambda
来源：http://www.m.share.hesvh.cn/Article/details/grxmbcaxm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.hesvh.cn/Article/details/gqoprfrkm.sHtML

[S46] C++：函数模板
来源：http://read.share.fehbvm.com/Article/details/gurbatlfj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fehbvm.com/Article/details/gqncnjstw.sHtML


<!-- 参考信息 -->