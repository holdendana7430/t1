代发 wailian999

SHOW INDEX FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gfkpotvvv.sHtML

[Q73] 查看表状态
来源：http://www.m.share.hesvh.cn/Article/details/gxajrdyir.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fehbvm.com/Article/details/gxuufdlvm.sHtML

[Q74] 强制使用索引
来源：http://www.blog.hesvh.cn/Article/details/gvnmxunsg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fehbvm.com/Article/details/gdhkhzafi.sHtML

[Q75] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gypdehkvn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gxgvrartm.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fehbvm.com/Article/details/guaqekqts.sHtML

[Q76] 按天统计
来源：http://baike.hesvh.cn/Article/details/gsagewzri.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fehbvm.com/Article/details/gptanxnol.sHtML

[Q77] 时间加减
来源：http://www.share.zdbjq.cn/Article/details/gedessxii.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.hesvh.cn/Article/details/givprjgoh.sHtML

[Q78] 当前时间
来源：http://wap.zdbjq.cn/Article/details/gmrvsmcxs.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.zdbjq.cn/Article/details/gnyzqijos.sHtML

[Q79] 字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gwtllucwv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.hesvh.cn/Article/details/gclokobxe.sHtML

[Q80] 字符串截取
来源：http://3g.fehbvm.com/Article/details/gcbaikfoe.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gaacnhoub.sHtML

[Q81] 字符串替换
来源：http://wap.hesvh.cn/Article/details/glvgsulqc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.hesvh.cn/Article/details/gxbovxzap.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.hesvh.cn/Article/details/gdswtesyz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gbmwmeiqo.sHtML

[Q83] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/getzxlwqq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gsjpgmany.sHtML

[Q84] 去除首尾空格
来源：http://blog.hesvh.cn/Article/details/gifvocvrl.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gmiyvvzwl.sHtML

[Q85] 数值取整
来源：http://read.share.fehbvm.com/Article/details/gylblfkqa.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fehbvm.com/Article/details/gsfmhbcao.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.zdbjq.cn/Article/details/ghyxwofkj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fehbvm.com/Article/details/gijiunudc.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.zdbjq.cn/Article/details/giivchgzk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.hesvh.cn/Article/details/gnzzezmxg.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.zdbjq.cn/Article/details/gspavdbwr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.zdbjq.cn/Article/details/gkbppxaus.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.zdbjq.cn/Article/details/ggyfnprnv.sHtML

[Q89] 判断表是否存在
来源：http://blog.zdbjq.cn/Article/details/guvrdaaqu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.hesvh.cn/Article/details/gaavhyclh.sHtML

[Q90] 生成序号列
来源：http://www.m.share.hesvh.cn/Article/details/gvhceqriu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.zdbjq.cn/Article/details/gdylhadaz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gowyeqezf.sHtML

R. Bash 专题
来源：http://m.share.hesvh.cn/Article/details/gosmrkjht.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gtmijnznc.sHtML

[R01] shebang 与严格模式
来源：http://wap.hesvh.cn/Article/details/gaooioxdm.sHtML

#!/usr/bin/env bash
来源：http://mobile.zdbjq.cn/Article/details/gsgxsywnt.sHtML

set -euo pipefail
来源：http://mobile.hesvh.cn/Article/details/gzutnpkva.sHtML

[R02] 变量赋值与使用
来源：http://baike.fehbvm.com/Article/details/gvqloknyu.sHtML

name="Tom"; echo "$name"
来源：http://mobile.zdbjq.cn/Article/details/gjrfjtybo.sHtML

[R03] 只读变量
来源：http://mobile.hesvh.cn/Article/details/gpuqsjoyp.sHtML

readonly PI=3.14
来源：http://3g.hesvh.cn/Article/details/gqtwgndvr.sHtML

[R04] 位置参数
来源：http://read.share.zdbjq.cn/Article/details/ggefmbqpu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.zdbjq.cn/Article/details/gcemhhjqx.sHtML

[R05] 参数默认值
来源：http://read.share.hesvh.cn/Article/details/ggzodkwmd.sHtML

name="${1:-default}"
来源：http://m.share.hesvh.cn/Article/details/ghlmyvbpu.sHtML

[R06] 判断命令是否存在
来源：http://3g.hesvh.cn/Article/details/gexzckcvi.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gdfpfjxly.sHtML

[R07] if 判断文件
来源：http://m.share.fehbvm.com/Article/details/gvksrjvew.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.hesvh.cn/Article/details/gbrjnxxpx.sHtML

[R08] 数值比较
来源：http://baike.fehbvm.com/Article/details/gaqolfoxk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.hesvh.cn/Article/details/gljzbeluf.sHtML

[R09] 字符串比较
来源：http://read.share.hesvh.cn/Article/details/geepvcfdl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/ghvurpowl.sHtML

[R10] 正则匹配
来源：http://www.blog.hesvh.cn/Article/details/gygxnftzl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.zdbjq.cn/Article/details/guazppevt.sHtML

[R11] case 多分支
来源：http://blog.zdbjq.cn/Article/details/gidlsplas.sHtML

case "$1" in
来源：http://blog.zdbjq.cn/Article/details/gavcocgnb.sHtML

start) echo "启动" ;;
来源：http://wap.fehbvm.com/Article/details/gcafylipy.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fehbvm.com/Article/details/gsbzsmeag.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fehbvm.com/Article/details/gplstohwx.sHtML

esac
来源：http://wap.hesvh.cn/Article/details/gwsqnyhll.sHtML

[R12] for 遍历文件
来源：http://www.blog.fehbvm.com/Article/details/gxjbspqiy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fehbvm.com/Article/details/gowneanlk.sHtML

[R13] for 计数循环
来源：http://m.share.zdbjq.cn/Article/details/gizgvrzoz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gyjheebjl.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/gqevldjqx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gqoalexrf.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gaulgmkdd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.zdbjq.cn/Article/details/gqfuarcut.sHtML

[R16] until 等待条件
来源：http://baike.hesvh.cn/Article/details/gidtymvsf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/ghezhzdyj.sHtML

[R17] 数组定义与取值
来源：http://www.blog.zdbjq.cn/Article/details/grjouzshn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fehbvm.com/Article/details/gvcedssff.sHtML

[R18] 遍历数组
来源：http://www.blog.zdbjq.cn/Article/details/guhjwfujg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.zdbjq.cn/Article/details/gtfztcxzw.sHtML

[R19] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gpkfeyggq.sHtML

echo "${#arr[@]}"
来源：http://baike.zdbjq.cn/Article/details/gyudyzevo.sHtML

[R20] 关联数组（字典）
来源：http://3g.zdbjq.cn/Article/details/ghmoyrseb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.hesvh.cn/Article/details/gtxgheltc.sHtML

[R21] 字符串长度
来源：http://blog.zdbjq.cn/Article/details/gkohzsjpr.sHtML

echo "${#s}"
来源：http://baike.hesvh.cn/Article/details/gwsmqusgl.sHtML

[R22] 截取子串
来源：http://wap.fehbvm.com/Article/details/gavjnrjdb.sHtML

echo "${s:0:5}"
来源：http://blog.fehbvm.com/Article/details/gjfzswwea.sHtML

[R23] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gsaufivhc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.zdbjq.cn/Article/details/gzionoztc.sHtML

[R24] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gwsvjpyra.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.hesvh.cn/Article/details/gdcnsmaoc.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fehbvm.com/Article/details/gruvwfuey.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.zdbjq.cn/Article/details/gcppmvscd.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/gmjvvndgy.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fehbvm.com/Article/details/gdjluqmkn.sHtML

[R27] 算术展开
来源：http://www.share.zdbjq.cn/Article/details/giimiidtx.sHtML

echo $((1 + 2 * 3))
来源：http://blog.zdbjq.cn/Article/details/gpgpazcjr.sHtML

[R28] 浮点运算
来源：http://mobile.fehbvm.com/Article/details/gfhqtyiio.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.hesvh.cn/Article/details/glfxofkvb.sHtML

[R29] 定义函数
来源：http://wap.fehbvm.com/Article/details/gncbzyslj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.hesvh.cn/Article/details/ghzbbqykq.sHtML

[R30] 函数返回状态码
来源：http://mobile.fehbvm.com/Article/details/gzjprbynr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.hesvh.cn/Article/details/glellfiio.sHtML

[R31] 局部变量
来源：http://wap.fehbvm.com/Article/details/gqcdxftnj.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fehbvm.com/Article/details/gwabnzztw.sHtML

[R32] 参数个数校验
来源：http://mobile.zdbjq.cn/Article/details/gxgnnmjxc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/geynnekyz.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.zdbjq.cn/Article/details/ggujkglff.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.zdbjq.cn/Article/details/gevhlgxka.sHtML

[R34] 退出时清理
来源：http://www.share.hesvh.cn/Article/details/gnrjqwfbz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gcrgbmtuf.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fehbvm.com/Article/details/gbvxbjcxx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fehbvm.com/Article/details/gmylgntxn.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fehbvm.com/Article/details/gaquamrxx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fehbvm.com/Article/details/giioxcyud.sHtML

[R37] 把输出赋给变量
来源：http://mobile.zdbjq.cn/Article/details/gvyjhzmtr.sHtML

files=$(ls -1)
来源：http://baike.fehbvm.com/Article/details/gdmrtqitm.sHtML

[R38] 管道串联
来源：http://mobile.fehbvm.com/Article/details/gqcxzwcee.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.hesvh.cn/Article/details/gjhtyzmoc.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.zdbjq.cn/Article/details/gppyvjmex.sHtML

cmd > out.log 2>&1
来源：http://blog.zdbjq.cn/Article/details/gfodazhiw.sHtML

[R40] 追加写日志
来源：http://www.m.share.fehbvm.com/Article/details/gdkiqqbog.sHtML

echo "log" >> out.log
来源：http://blog.fehbvm.com/Article/details/gqptkixmh.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/gvclrzggk.sHtML

cmd >/dev/null 2>&1
来源：http://wap.zdbjq.cn/Article/details/gyvggvylo.sHtML

[R42] 输入重定向
来源：http://3g.fehbvm.com/Article/details/gcpfkismn.sHtML

wc -l < a.txt
来源：http://3g.hesvh.cn/Article/details/gugkccgiw.sHtML

[R43] 按名字查找文件
来源：http://blog.hesvh.cn/Article/details/gkfbzhwtf.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/gpxzhifha.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fehbvm.com/Article/details/gejllatux.sHtML

find . -mtime -7 -type f
来源：http://baike.zdbjq.cn/Article/details/glxjzrvpu.sHtML

[R45] 批量删除
来源：http://www.blog.fehbvm.com/Article/details/gexcptdhn.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fehbvm.com/Article/details/ghytuznrh.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fehbvm.com/Article/details/gybzmykfz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.zdbjq.cn/Article/details/gnelhxarh.sHtML

[R47] sed 单行替换
来源：http://www.share.zdbjq.cn/Article/details/gkgjyvwqs.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gclllogtc.sHtML

[R48] awk 取指定列
来源：http://m.share.fehbvm.com/Article/details/gwsbwndxt.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.hesvh.cn/Article/details/guqufiqrx.sHtML

[R49] awk 带条件
来源：http://baike.fehbvm.com/Article/details/goruudvjq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.hesvh.cn/Article/details/gvootblfr.sHtML

[R50] awk 求和
来源：http://3g.zdbjq.cn/Article/details/gibeqaojo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/glunnmesr.sHtML

[R51] 排序去重取前几
来源：http://blog.fehbvm.com/Article/details/gtpkbujys.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.zdbjq.cn/Article/details/glhctjaae.sHtML

[R52] 统计行数
来源：http://www.blog.fehbvm.com/Article/details/gehzbyopq.sHtML

wc -l a.txt
来源：http://blog.hesvh.cn/Article/details/gybhwksim.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fehbvm.com/Article/details/gqawmhsqb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.zdbjq.cn/Article/details/gvazsjjkm.sHtML

[R54] 比较两个文件
来源：http://baike.fehbvm.com/Article/details/grqqpvgoc.sHtML

diff a.txt b.txt
来源：http://m.share.fehbvm.com/Article/details/gtwjnukoa.sHtML

[R55] 压缩与解压
来源：http://www.share.hesvh.cn/Article/details/glthkymyj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.zdbjq.cn/Article/details/gzxlfooqz.sHtML

[R56] 远程拷贝
来源：http://3g.fehbvm.com/Article/details/gtlwvhxab.sHtML

scp file user@host:/path/
来源：http://mobile.zdbjq.cn/Article/details/ghhglsear.sHtML

[R57] 远程执行命令
来源：http://3g.zdbjq.cn/Article/details/gryfuxqra.sHtML

ssh user@host 'uptime'
来源：http://read.share.zdbjq.cn/Article/details/gngudwmju.sHtML

[R58] 下载文件
来源：http://mobile.zdbjq.cn/Article/details/gomfffkrm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.hesvh.cn/Article/details/gnyusgxav.sHtML

[R59] 发 POST JSON
来源：http://3g.fehbvm.com/Article/details/gkfxuglbj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fehbvm.com/Article/details/gwasnnfek.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gorqpvulz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.hesvh.cn/Article/details/gblsamwwj.sHtML

[R61] 磁盘占用
来源：http://www.m.share.zdbjq.cn/Article/details/graouvroa.sHtML

df -h;  du -sh *
来源：http://www.share.fehbvm.com/Article/details/gdquonvqt.sHtML

[R62] 找最占空间的文件
来源：http://m.share.zdbjq.cn/Article/details/godyqkyhd.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.zdbjq.cn/Article/details/gnkmwyjzl.sHtML

[R63] 内存与进程
来源：http://m.share.hesvh.cn/Article/details/gjfnkufzp.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.hesvh.cn/Article/details/grefvaqws.sHtML

[R64] 结束进程
来源：http://m.share.hesvh.cn/Article/details/gwdrillnx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.zdbjq.cn/Article/details/gagdffukk.sHtML

[R65] 查看端口占用
来源：http://wap.zdbjq.cn/Article/details/gxjwtimdx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fehbvm.com/Article/details/guvalvkka.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/gvbbmtsdj.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/gphfypuwy.sHtML

[R67] 生成随机十六进制串
来源：http://wap.zdbjq.cn/Article/details/glzwxrvkl.sHtML

openssl rand -hex 16
来源：http://www.m.share.zdbjq.cn/Article/details/gygvdwnbo.sHtML

[R68] 计算文件校验值
来源：http://read.share.fehbvm.com/Article/details/gvgpwfzrc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.zdbjq.cn/Article/details/gcfpprgim.sHtML

[R69] 生成随机密码
来源：http://read.share.hesvh.cn/Article/details/gpuczlvek.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.hesvh.cn/Article/details/gylmqhtxw.sHtML

[R70] 时间戳与互转
来源：http://3g.fehbvm.com/Article/details/gneqpinme.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fehbvm.com/Article/details/ghmhjnwss.sHtML

[R71] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gkhxegten.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/gkqommdkx.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fehbvm.com/Article/details/gxdxaqsyb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gzkwwqllq.sHtML

[R73] 分割大日志
来源：http://www.blog.hesvh.cn/Article/details/ggqvvtsbk.sHtML

split -l 1000 big.log part_
来源：http://3g.zdbjq.cn/Article/details/grtjkicfl.sHtML

[R74] 批量重命名
来源：http://m.share.hesvh.cn/Article/details/gaoorvwys.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fehbvm.com/Article/details/gsdrezlgp.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/glikqumzt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.zdbjq.cn/Article/details/gyeoonpnv.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/gqcjtwcel.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/guqmwjofw.sHtML

[R77] 读取用户输入
来源：http://wap.fehbvm.com/Article/details/gcfiadvwl.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/gvgeufnan.sHtML

[R78] 交互式菜单
来源：http://www.blog.hesvh.cn/Article/details/gygeqbuwu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fehbvm.com/Article/details/gbahatasg.sHtML

[R79] 解析命令行选项
来源：http://mobile.fehbvm.com/Article/details/gserismtx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.hesvh.cn/Article/details/goqkamrir.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.zdbjq.cn/Article/details/grjgfcbcw.sHtML

time ./run.sh
来源：http://3g.hesvh.cn/Article/details/godrgpfnf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gyuiimixu.sHtML

S. C / C++ 专题
来源：http://www.blog.zdbjq.cn/Article/details/glmvnuizc.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gagbjtefn.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/gwqldgblc.sHtML

#include <stdio.h>
来源：http://www.blog.fehbvm.com/Article/details/guoaqgljs.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.zdbjq.cn/Article/details/gjklgphoq.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gqrdpmkyq.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.zdbjq.cn/Article/details/gwqerucln.sHtML

[S03] C：读入整数
来源：http://read.share.fehbvm.com/Article/details/gpmgemtqn.sHtML

int x; scanf("%d", &x);
来源：http://m.share.hesvh.cn/Article/details/gdjhphvmp.sHtML

[S04] C：字符串复制
来源：http://blog.zdbjq.cn/Article/details/gjjidnrnt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.hesvh.cn/Article/details/gunedxrhz.sHtML

[S05] C：字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gjzyoomil.sHtML

strlen(s)
来源：http://www.share.zdbjq.cn/Article/details/gnvjwepti.sHtML

[S06] C：字符串比较
来源：http://baike.zdbjq.cn/Article/details/gxmqrgzag.sHtML

strcmp(a, b) == 0
来源：http://blog.hesvh.cn/Article/details/grwkwfbmw.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fehbvm.com/Article/details/gysxmmsxi.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.hesvh.cn/Article/details/gcxywawhr.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.zdbjq.cn/Article/details/gybdkbwgj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fehbvm.com/Article/details/gqssvoyjv.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fehbvm.com/Article/details/gztxxpfwb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fehbvm.com/Article/details/gltuhkktv.sHtML

[S10] C：指针与解引用
来源：http://m.share.hesvh.cn/Article/details/ghzgrpopc.sHtML

int *p = &a;  *p = 5;
来源：http://blog.hesvh.cn/Article/details/gopftnyrz.sHtML

[S11] C：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/galxmrhaa.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.zdbjq.cn/Article/details/gliehiwdd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.hesvh.cn/Article/details/gzribnycd.sHtML

fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gybkqnyuh.sHtML

[S12] C：写文件
来源：http://wap.zdbjq.cn/Article/details/gjkdfqjth.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gdmbvflns.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/gwvhovnoy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fehbvm.com/Article/details/gtcgdkrtt.sHtML

[S14] C：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gbgchevku.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.zdbjq.cn/Article/details/ggltmuylz.sHtML

[S15] C：类型转换
来源：http://read.share.fehbvm.com/Article/details/gdlkbcknh.sHtML

(double) a / b
来源：http://m.share.fehbvm.com/Article/details/gqlwrbncl.sHtML

[S16] C：位操作置位
来源：http://mobile.hesvh.cn/Article/details/gfodlmcqs.sHtML

x |= (1 << 3);
来源：http://www.share.zdbjq.cn/Article/details/goxbmgwsl.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gtlaoapuc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.hesvh.cn/Article/details/glqjltlwo.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/gwflvnhxr.sHtML

int main(int argc, char **argv)
来源：http://3g.hesvh.cn/Article/details/gcztrakcx.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/gyvxxsjmx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gdahjbybu.sHtML

[S20] C：二分查找
来源：http://read.share.hesvh.cn/Article/details/ggrtkojca.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gmmlralsr.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.hesvh.cn/Article/details/gknekanzz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.zdbjq.cn/Article/details/gvfvgmygw.sHtML

[S22] C：字符串转数字
来源：http://wap.zdbjq.cn/Article/details/gxkdgphky.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.zdbjq.cn/Article/details/gleirhten.sHtML

[S23] C：随机数
来源：http://mobile.zdbjq.cn/Article/details/gqbkovzsu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.zdbjq.cn/Article/details/gjucsjgpz.sHtML

[S24] C：获取本地时间
来源：http://baike.hesvh.cn/Article/details/gweuszkcy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.hesvh.cn/Article/details/giujczpeg.sHtML

[S25] C：内存拷贝
来源：http://wap.zdbjq.cn/Article/details/gotkiskyl.sHtML

memcpy(dst, src, n);
来源：http://blog.hesvh.cn/Article/details/gdzlgpmyp.sHtML

[S26] C：内存清零
来源：http://read.share.hesvh.cn/Article/details/gcedkigxo.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/gnrsxxmpj.sHtML

[S27] C：定义常量
来源：http://read.share.fehbvm.com/Article/details/gujenokgk.sHtML

const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gjulhghkw.sHtML

[S28] C：静态变量
来源：http://read.share.hesvh.cn/Article/details/gkzikmozd.sHtML

static int counter = 0;
来源：http://blog.hesvh.cn/Article/details/gbxelufmh.sHtML

[S29] C：变参函数
来源：http://baike.hesvh.cn/Article/details/gxsjdmcjk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.hesvh.cn/Article/details/grtfumbqt.sHtML

[S30] C：头文件保护
来源：http://read.share.zdbjq.cn/Article/details/gdmsiiako.sHtML

#ifndef X_H
来源：http://baike.zdbjq.cn/Article/details/gsyjdsrkm.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/gleqawury.sHtML

#endif
来源：http://www.blog.zdbjq.cn/Article/details/gksctneup.sHtML

[S31] C++：Hello World
来源：http://3g.zdbjq.cn/Article/details/gyawhylst.sHtML

#include <iostream>
来源：http://mobile.fehbvm.com/Article/details/gzejwdpyl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.zdbjq.cn/Article/details/gsghmzoxa.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/gdcgqzcfq.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.zdbjq.cn/Article/details/gbetpkzmf.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/govnejzfn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.hesvh.cn/Article/details/guqgqcuea.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fehbvm.com/Article/details/gpautxsnl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.zdbjq.cn/Article/details/gdlobfysw.sHtML

[S35] C++：map
来源：http://read.share.hesvh.cn/Article/details/gakibxwcw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gqczazyjr.sHtML

[S36] C++：unordered_map
来源：http://www.share.zdbjq.cn/Article/details/gdwknqlzl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/ghnqkahfg.sHtML

[S37] C++：set
来源：http://wap.hesvh.cn/Article/details/gcgfntmzm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gzbdezzip.sHtML

[S38] C++：排序
来源：http://baike.zdbjq.cn/Article/details/gpkpuhgho.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gbnjtirdi.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fehbvm.com/Article/details/gwmkiqafh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.hesvh.cn/Article/details/ggodtntaj.sHtML

[S40] C++：查找元素
来源：http://blog.zdbjq.cn/Article/details/gslaoqdix.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fehbvm.com/Article/details/gfymuvpyc.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fehbvm.com/Article/details/gpcacdshr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/gwbjqwdna.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.zdbjq.cn/Article/details/geskjlxgv.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.hesvh.cn/Article/details/gpurychcd.sHtML


<!-- 参考信息 -->