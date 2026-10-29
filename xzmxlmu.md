代发 wailian999

[Q76] 按天统计
来源：http://m.share.hesvh.cn/Article/details/glgkunaef.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.zdbjq.cn/Article/details/gzprdyhwq.sHtML

[Q77] 时间加减
来源：http://wap.hesvh.cn/Article/details/gcqbkyacw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fehbvm.com/Article/details/gmyajjlcu.sHtML

[Q78] 当前时间
来源：http://www.blog.fehbvm.com/Article/details/gjrdqzyoi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.hesvh.cn/Article/details/gtlldvqzm.sHtML

[Q79] 字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gmxjvkpbm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.hesvh.cn/Article/details/gsziodqvj.sHtML

[Q80] 字符串截取
来源：http://baike.fehbvm.com/Article/details/gwwbqgdrb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/guihcazni.sHtML

[Q81] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gepzsecvi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fehbvm.com/Article/details/ggiepjrqt.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fehbvm.com/Article/details/ggoororrm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/goowwkkph.sHtML

[Q83] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gmvhlqrfn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gfxlmxkxu.sHtML

[Q84] 去除首尾空格
来源：http://read.share.hesvh.cn/Article/details/gcxpaolyz.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gehdpuzyg.sHtML

[Q85] 数值取整
来源：http://wap.fehbvm.com/Article/details/gpgxcasbm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fehbvm.com/Article/details/gveejcpit.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.zdbjq.cn/Article/details/gxuhzkujh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fehbvm.com/Article/details/ghjhlhtlu.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fehbvm.com/Article/details/gdgdrzclk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fehbvm.com/Article/details/gpglhuekq.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fehbvm.com/Article/details/gjfcplrfn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fehbvm.com/Article/details/gmwpwcilo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.hesvh.cn/Article/details/gdztwepyn.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gcbhttojx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.zdbjq.cn/Article/details/giofogirq.sHtML

[Q90] 生成序号列
来源：http://www.blog.hesvh.cn/Article/details/gipxwtiis.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fehbvm.com/Article/details/gxubqiqyz.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gadmmzmuu.sHtML

R. Bash 专题
来源：http://www.m.share.hesvh.cn/Article/details/gqaixwgsj.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gifvuxdoi.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.hesvh.cn/Article/details/gumrtugip.sHtML

#!/usr/bin/env bash
来源：http://read.share.zdbjq.cn/Article/details/gnwjnqbnj.sHtML

set -euo pipefail
来源：http://baike.hesvh.cn/Article/details/ggciskduj.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fehbvm.com/Article/details/gmwxhjplg.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.zdbjq.cn/Article/details/giulnjjuh.sHtML

[R03] 只读变量
来源：http://m.share.zdbjq.cn/Article/details/gmkupibha.sHtML

readonly PI=3.14
来源：http://mobile.zdbjq.cn/Article/details/ghzelfipp.sHtML

[R04] 位置参数
来源：http://mobile.hesvh.cn/Article/details/gcdauexdl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.zdbjq.cn/Article/details/gxtnsatbg.sHtML

[R05] 参数默认值
来源：http://wap.fehbvm.com/Article/details/gdaujbrqp.sHtML

name="${1:-default}"
来源：http://www.share.hesvh.cn/Article/details/gikpcjjnj.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.hesvh.cn/Article/details/glmupbbec.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gjuyxvdkl.sHtML

[R07] if 判断文件
来源：http://wap.hesvh.cn/Article/details/gvdomxsba.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/gsrgtvdzp.sHtML

[R08] 数值比较
来源：http://www.blog.hesvh.cn/Article/details/gbuzkteda.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.zdbjq.cn/Article/details/glebuhwip.sHtML

[R09] 字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gmslxkutw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.hesvh.cn/Article/details/gvoykjdqu.sHtML

[R10] 正则匹配
来源：http://www.blog.zdbjq.cn/Article/details/geqwjltxx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.hesvh.cn/Article/details/gfhuonozt.sHtML

[R11] case 多分支
来源：http://mobile.hesvh.cn/Article/details/gupdtfojy.sHtML

case "$1" in
来源：http://www.m.share.hesvh.cn/Article/details/gktadjppb.sHtML

start) echo "启动" ;;
来源：http://wap.hesvh.cn/Article/details/gicfgrdpm.sHtML

stop)  echo "停止" ;;
来源：http://blog.hesvh.cn/Article/details/geunggiqk.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.zdbjq.cn/Article/details/gxyaasawo.sHtML

esac
来源：http://3g.fehbvm.com/Article/details/gnudqokpa.sHtML

[R12] for 遍历文件
来源：http://m.share.hesvh.cn/Article/details/ggtqllska.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.zdbjq.cn/Article/details/ghhohwgtk.sHtML

[R13] for 计数循环
来源：http://read.share.zdbjq.cn/Article/details/ghfxtgztu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gfnvvalmb.sHtML

[R14] C 风格 for
来源：http://wap.hesvh.cn/Article/details/gjfnpfthy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/grbbcmnlj.sHtML

[R15] while 逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gxymihsxj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fehbvm.com/Article/details/gadtgnuqg.sHtML

[R16] until 等待条件
来源：http://www.m.share.hesvh.cn/Article/details/gqohaikrl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gzbnaihqr.sHtML

[R17] 数组定义与取值
来源：http://mobile.hesvh.cn/Article/details/gbggmnzhi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.hesvh.cn/Article/details/gjqnpdprs.sHtML

[R18] 遍历数组
来源：http://m.share.fehbvm.com/Article/details/gegbleezi.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/gaxeapleb.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gkonlfupn.sHtML

echo "${#arr[@]}"
来源：http://read.share.hesvh.cn/Article/details/gizmzmdwc.sHtML

[R20] 关联数组（字典）
来源：http://read.share.hesvh.cn/Article/details/gpgaerdyk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.hesvh.cn/Article/details/gcydnzelr.sHtML

[R21] 字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gnwdegtyg.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/gxmwyvopt.sHtML

[R22] 截取子串
来源：http://read.share.hesvh.cn/Article/details/ghvhpprmo.sHtML

echo "${s:0:5}"
来源：http://blog.zdbjq.cn/Article/details/gsfhfwsng.sHtML

[R23] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gjacwepsk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.hesvh.cn/Article/details/gauhhwena.sHtML

[R24] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gwjeplxzr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.zdbjq.cn/Article/details/gzfldcbuo.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.zdbjq.cn/Article/details/gfwyikbqf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.zdbjq.cn/Article/details/gjlgilaju.sHtML

[R26] 命令替换
来源：http://baike.zdbjq.cn/Article/details/gdvktlbew.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.hesvh.cn/Article/details/gnsnjgaem.sHtML

[R27] 算术展开
来源：http://www.blog.hesvh.cn/Article/details/gwrrnsksx.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fehbvm.com/Article/details/glnkaclin.sHtML

[R28] 浮点运算
来源：http://blog.zdbjq.cn/Article/details/gtcbxcbzx.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fehbvm.com/Article/details/gjbunttbs.sHtML

[R29] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gkfauavxa.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.zdbjq.cn/Article/details/giekgzlyb.sHtML

[R30] 函数返回状态码
来源：http://www.share.zdbjq.cn/Article/details/gamlakmfr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.zdbjq.cn/Article/details/gumjgiznk.sHtML

[R31] 局部变量
来源：http://www.share.hesvh.cn/Article/details/ghngzmiiz.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fehbvm.com/Article/details/gckwpupjs.sHtML

[R32] 参数个数校验
来源：http://www.m.share.zdbjq.cn/Article/details/gvletnbgv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/ghlfzjrwp.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fehbvm.com/Article/details/gpklihnvf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.zdbjq.cn/Article/details/geufkeduc.sHtML

[R34] 退出时清理
来源：http://blog.hesvh.cn/Article/details/gpowuhmtc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gsujajwds.sHtML

[R35] 后台执行并等待
来源：http://read.share.fehbvm.com/Article/details/grwyejugm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.zdbjq.cn/Article/details/gickwxfwn.sHtML

[R36] 并发执行多个任务
来源：http://m.share.hesvh.cn/Article/details/gyjqrxige.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.zdbjq.cn/Article/details/gxnapniyf.sHtML

[R37] 把输出赋给变量
来源：http://m.share.zdbjq.cn/Article/details/gbawbhvlx.sHtML

files=$(ls -1)
来源：http://blog.hesvh.cn/Article/details/gspqhxmah.sHtML

[R38] 管道串联
来源：http://baike.zdbjq.cn/Article/details/glzofasil.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.hesvh.cn/Article/details/gondbetfz.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.hesvh.cn/Article/details/gtqnwnoce.sHtML

cmd > out.log 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gvyymjhvn.sHtML

[R40] 追加写日志
来源：http://m.share.fehbvm.com/Article/details/gvjzffydc.sHtML

echo "log" >> out.log
来源：http://mobile.fehbvm.com/Article/details/gjeupqwit.sHtML

[R41] 丢弃输出
来源：http://3g.fehbvm.com/Article/details/gudiacsle.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gacthmcmc.sHtML

[R42] 输入重定向
来源：http://www.m.share.hesvh.cn/Article/details/gejthfyyo.sHtML

wc -l < a.txt
来源：http://blog.zdbjq.cn/Article/details/ghgkugpto.sHtML

[R43] 按名字查找文件
来源：http://www.blog.hesvh.cn/Article/details/gnvvxadcl.sHtML

find . -name "*.log" -type f
来源：http://3g.fehbvm.com/Article/details/grmbtyqvx.sHtML

[R44] 按修改时间查找
来源：http://www.blog.zdbjq.cn/Article/details/gwrfngopd.sHtML

find . -mtime -7 -type f
来源：http://baike.hesvh.cn/Article/details/gdzqjmjnm.sHtML

[R45] 批量删除
来源：http://read.share.fehbvm.com/Article/details/giwctwpqz.sHtML

find . -name "*.tmp" -delete
来源：http://blog.hesvh.cn/Article/details/gqsivbjym.sHtML

[R46] 递归替换文件内容
来源：http://blog.hesvh.cn/Article/details/gfvftrkps.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.hesvh.cn/Article/details/gezhsdzys.sHtML

[R47] sed 单行替换
来源：http://www.share.hesvh.cn/Article/details/gcljzegoz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/godwxnvhk.sHtML

[R48] awk 取指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gelsiafft.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gevddnzhi.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/gxigkpnom.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.zdbjq.cn/Article/details/gymqjfcrv.sHtML

[R50] awk 求和
来源：http://www.share.fehbvm.com/Article/details/ghhnxukfx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/gbefsbjqe.sHtML

[R51] 排序去重取前几
来源：http://www.share.fehbvm.com/Article/details/gpevukiub.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.hesvh.cn/Article/details/gzheepzgp.sHtML

[R52] 统计行数
来源：http://blog.hesvh.cn/Article/details/gsgeccyga.sHtML

wc -l a.txt
来源：http://baike.hesvh.cn/Article/details/glohdzyjw.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.zdbjq.cn/Article/details/gfzskkhsv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.hesvh.cn/Article/details/gmwzyqovx.sHtML

[R54] 比较两个文件
来源：http://www.share.hesvh.cn/Article/details/gamxauqig.sHtML

diff a.txt b.txt
来源：http://m.share.hesvh.cn/Article/details/gqaadtsuu.sHtML

[R55] 压缩与解压
来源：http://m.share.hesvh.cn/Article/details/ggqykhrqh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.hesvh.cn/Article/details/gpnumccin.sHtML

[R56] 远程拷贝
来源：http://blog.zdbjq.cn/Article/details/gvmupxncb.sHtML

scp file user@host:/path/
来源：http://www.blog.fehbvm.com/Article/details/gszetjufo.sHtML

[R57] 远程执行命令
来源：http://m.share.hesvh.cn/Article/details/gzoevhjfj.sHtML

ssh user@host 'uptime'
来源：http://3g.fehbvm.com/Article/details/gcfwboome.sHtML

[R58] 下载文件
来源：http://m.share.fehbvm.com/Article/details/ggcwezmui.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.zdbjq.cn/Article/details/gcwvolguk.sHtML

[R59] 发 POST JSON
来源：http://blog.hesvh.cn/Article/details/gbrrqyqll.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.hesvh.cn/Article/details/guyfakcnz.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gvnfikopn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/glfakmfsp.sHtML

[R61] 磁盘占用
来源：http://wap.fehbvm.com/Article/details/ggqzaebmk.sHtML

df -h;  du -sh *
来源：http://read.share.fehbvm.com/Article/details/gtspsyemf.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fehbvm.com/Article/details/gytjuncmn.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.zdbjq.cn/Article/details/gaqfgftse.sHtML

[R63] 内存与进程
来源：http://read.share.zdbjq.cn/Article/details/grbjlntlm.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.hesvh.cn/Article/details/guoeukxee.sHtML

[R64] 结束进程
来源：http://read.share.hesvh.cn/Article/details/gkiyvnxsl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/gdusbjmbr.sHtML

[R65] 查看端口占用
来源：http://3g.fehbvm.com/Article/details/gegnqmnjp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.zdbjq.cn/Article/details/gmliwvlqm.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gfelleson.sHtML

crontab -e;  crontab -l
来源：http://www.share.hesvh.cn/Article/details/gohyujljn.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/givtcjtwt.sHtML

openssl rand -hex 16
来源：http://mobile.fehbvm.com/Article/details/ghtjgqmwh.sHtML

[R68] 计算文件校验值
来源：http://m.share.fehbvm.com/Article/details/gebjxmcog.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.hesvh.cn/Article/details/gwwdxzuqs.sHtML

[R69] 生成随机密码
来源：http://m.share.fehbvm.com/Article/details/gouxpbsmi.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.zdbjq.cn/Article/details/gniimntjc.sHtML

[R70] 时间戳与互转
来源：http://www.share.fehbvm.com/Article/details/gdmybxgui.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.hesvh.cn/Article/details/gwqhzblmd.sHtML

[R71] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gmhwgxxwi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.hesvh.cn/Article/details/gikuhawzn.sHtML

[R72] 等待端口就绪
来源：http://m.share.fehbvm.com/Article/details/gzgrgsejc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gdnnikxkc.sHtML

[R73] 分割大日志
来源：http://m.share.zdbjq.cn/Article/details/glqfjzjwa.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.zdbjq.cn/Article/details/gvmixmyfa.sHtML

[R74] 批量重命名
来源：http://3g.hesvh.cn/Article/details/gtfzwajfk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.hesvh.cn/Article/details/glyrwfxyi.sHtML

[R75] 导出环境变量
来源：http://www.blog.hesvh.cn/Article/details/gybtoqcgz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fehbvm.com/Article/details/gruwuvdif.sHtML

[R76] 使用临时文件
来源：http://www.m.share.hesvh.cn/Article/details/gynkautvq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gdfizrjsb.sHtML

[R77] 读取用户输入
来源：http://m.share.hesvh.cn/Article/details/gerewuzfi.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.zdbjq.cn/Article/details/gbhxyyemy.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/gfyehmgss.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fehbvm.com/Article/details/gdnwekbje.sHtML

[R79] 解析命令行选项
来源：http://www.share.zdbjq.cn/Article/details/gyixyyunr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fehbvm.com/Article/details/grlvbazrm.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.hesvh.cn/Article/details/gsbpmhawa.sHtML

time ./run.sh
来源：http://www.share.hesvh.cn/Article/details/gnkxunhbt.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/geahxzoyz.sHtML

S. C / C++ 专题
来源：http://www.blog.fehbvm.com/Article/details/gvndurrqx.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtthfhljf.sHtML

[S01] C：Hello World
来源：http://baike.hesvh.cn/Article/details/gxcmffqvu.sHtML

#include <stdio.h>
来源：http://blog.zdbjq.cn/Article/details/gulwpovxu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.hesvh.cn/Article/details/gwuihllha.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.hesvh.cn/Article/details/grvnidlpi.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.zdbjq.cn/Article/details/gnrjdsgtr.sHtML

[S03] C：读入整数
来源：http://3g.zdbjq.cn/Article/details/gaxsqbzeb.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/ghokltmco.sHtML

[S04] C：字符串复制
来源：http://3g.fehbvm.com/Article/details/gtoqahgtp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fehbvm.com/Article/details/gijqvtswk.sHtML

[S05] C：字符串长度
来源：http://3g.fehbvm.com/Article/details/gzurphglr.sHtML

strlen(s)
来源：http://www.blog.fehbvm.com/Article/details/ggyikjnyv.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/guwemtpfk.sHtML

strcmp(a, b) == 0
来源：http://read.share.hesvh.cn/Article/details/gaslujvcx.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fehbvm.com/Article/details/gliihbrmy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.zdbjq.cn/Article/details/glskgkgji.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fehbvm.com/Article/details/gkthecixl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/gxnktlmaz.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.hesvh.cn/Article/details/gpxiyukdd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fehbvm.com/Article/details/gvljktbyb.sHtML

[S10] C：指针与解引用
来源：http://www.share.fehbvm.com/Article/details/gsuutosmc.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fehbvm.com/Article/details/gifhuzllb.sHtML

[S11] C：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/geyjxomca.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fehbvm.com/Article/details/ggsezadzn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.hesvh.cn/Article/details/gbbnalkxz.sHtML

fclose(f);
来源：http://3g.fehbvm.com/Article/details/gfcqlclxo.sHtML

[S12] C：写文件
来源：http://baike.zdbjq.cn/Article/details/gvbpticaj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/ggiwzlrss.sHtML

[S13] C：宏定义
来源：http://www.m.share.fehbvm.com/Article/details/gmnsknmqa.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fehbvm.com/Article/details/gwkndbjwl.sHtML

[S14] C：枚举
来源：http://3g.hesvh.cn/Article/details/ggkwuexwt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.hesvh.cn/Article/details/ggklxdmbe.sHtML

[S15] C：类型转换
来源：http://mobile.fehbvm.com/Article/details/gyydvulbh.sHtML

(double) a / b
来源：http://www.m.share.zdbjq.cn/Article/details/gjejqypcv.sHtML

[S16] C：位操作置位
来源：http://m.share.fehbvm.com/Article/details/gklwolzzh.sHtML

x |= (1 << 3);
来源：http://mobile.hesvh.cn/Article/details/gbxmprvys.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.hesvh.cn/Article/details/glxykwhwq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.zdbjq.cn/Article/details/geisyheob.sHtML

[S18] C：命令行参数
来源：http://wap.fehbvm.com/Article/details/gmxrzatgy.sHtML

int main(int argc, char **argv)
来源：http://3g.fehbvm.com/Article/details/ggddojmrz.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/gwolfjzuk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gjyrtbawu.sHtML

[S20] C：二分查找
来源：http://3g.hesvh.cn/Article/details/gglukzqwn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gpqlogsut.sHtML

[S21] C：字符类别判断
来源：http://3g.hesvh.cn/Article/details/gieexpbyw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fehbvm.com/Article/details/grqbeodbc.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/ggrbjllhh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.hesvh.cn/Article/details/gjxtyqvdi.sHtML

[S23] C：随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gtcznjlxs.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.hesvh.cn/Article/details/ghcplwboc.sHtML

[S24] C：获取本地时间
来源：http://blog.hesvh.cn/Article/details/gxznrxfyu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.zdbjq.cn/Article/details/gmusrlfkf.sHtML

[S25] C：内存拷贝
来源：http://baike.zdbjq.cn/Article/details/guzgwuvie.sHtML

memcpy(dst, src, n);
来源：http://wap.hesvh.cn/Article/details/guqqkcwgu.sHtML

[S26] C：内存清零
来源：http://3g.hesvh.cn/Article/details/ghpvphalb.sHtML

memset(a, 0, sizeof a);
来源：http://blog.hesvh.cn/Article/details/gtxtolfnc.sHtML

[S27] C：定义常量
来源：http://blog.zdbjq.cn/Article/details/gpewekbju.sHtML

const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gjqpluykj.sHtML

[S28] C：静态变量
来源：http://www.m.share.hesvh.cn/Article/details/gxvtoyplt.sHtML

static int counter = 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gsunvacqk.sHtML

[S29] C：变参函数
来源：http://m.share.fehbvm.com/Article/details/gprtjvbwv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/gzqcqtpzw.sHtML

[S30] C：头文件保护
来源：http://www.blog.zdbjq.cn/Article/details/gnoafaddp.sHtML

#ifndef X_H
来源：http://baike.fehbvm.com/Article/details/getsgekoy.sHtML

#define X_H
来源：http://blog.zdbjq.cn/Article/details/gzbouloyj.sHtML

#endif
来源：http://read.share.hesvh.cn/Article/details/gtbjewmza.sHtML

[S31] C++：Hello World
来源：http://blog.zdbjq.cn/Article/details/gjadmrwlh.sHtML

#include <iostream>
来源：http://www.share.fehbvm.com/Article/details/gvesbqrdf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/gdneljkpd.sHtML

[S32] C++：字符串
来源：http://baike.zdbjq.cn/Article/details/gjgsjdqpv.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fehbvm.com/Article/details/gvgfmfiva.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/gaqqrcfto.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gaexyhryr.sHtML

[S34] C++：遍历 vector
来源：http://baike.hesvh.cn/Article/details/gauqvifzv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.hesvh.cn/Article/details/gufcogsxe.sHtML

[S35] C++：map
来源：http://www.blog.fehbvm.com/Article/details/gazyhugcs.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gopclixen.sHtML

[S36] C++：unordered_map
来源：http://3g.hesvh.cn/Article/details/gfslhigma.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gyvtmxxdm.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/gjrdbezbx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.zdbjq.cn/Article/details/gqwnicmzi.sHtML

[S38] C++：排序
来源：http://read.share.hesvh.cn/Article/details/gjhhfxsjo.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/girhhzhxj.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fehbvm.com/Article/details/gbykrlgra.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fehbvm.com/Article/details/gmynpvnce.sHtML

[S40] C++：查找元素
来源：http://3g.fehbvm.com/Article/details/gyrhgaajq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fehbvm.com/Article/details/gvhenrlpm.sHtML

[S41] C++：类与构造函数
来源：http://blog.fehbvm.com/Article/details/grpnpylev.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.zdbjq.cn/Article/details/glwwriuql.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.hesvh.cn/Article/details/gpifukcrj.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fehbvm.com/Article/details/gjnrpwgdn.sHtML

[S43] C++：智能指针
来源：http://www.share.zdbjq.cn/Article/details/gokyeoqrj.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/gdysefyky.sHtML

[S44] C++：引用传参
来源：http://3g.hesvh.cn/Article/details/gragcienf.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/guwchtqjh.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/gyrlfhdqe.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/ggemnyhco.sHtML

[S46] C++：函数模板
来源：http://www.m.share.hesvh.cn/Article/details/grkvvlwir.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.zdbjq.cn/Article/details/grhxspvbb.sHtML


<!-- 参考信息 -->