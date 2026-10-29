代发 wailian999

[Q84] 去除首尾空格
来源：http://m.share.zdbjq.cn/Article/details/gdkijkdss.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gfjirfmvl.sHtML

[Q85] 数值取整
来源：http://m.share.fehbvm.com/Article/details/gsjipvspi.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.zdbjq.cn/Article/details/ghowegbrf.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.hesvh.cn/Article/details/grhqsfrin.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fehbvm.com/Article/details/gfnbxmbjc.sHtML

[Q87] JSON 字段做条件
来源：http://blog.hesvh.cn/Article/details/gcmuqbesn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.zdbjq.cn/Article/details/gjuvffhdq.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.hesvh.cn/Article/details/gpavmihuv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.zdbjq.cn/Article/details/gwvufpnbn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gteoxycvr.sHtML

[Q89] 判断表是否存在
来源：http://baike.hesvh.cn/Article/details/gynombruj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.zdbjq.cn/Article/details/giqqryejv.sHtML

[Q90] 生成序号列
来源：http://wap.fehbvm.com/Article/details/gclbmlpnu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.hesvh.cn/Article/details/glvdlgutz.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gbcbotley.sHtML

R. Bash 专题
来源：http://baike.hesvh.cn/Article/details/guigzmyza.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gybxsjyvk.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.zdbjq.cn/Article/details/guxvzrids.sHtML

#!/usr/bin/env bash
来源：http://read.share.zdbjq.cn/Article/details/geivofjgx.sHtML

set -euo pipefail
来源：http://www.share.zdbjq.cn/Article/details/givjlzeza.sHtML

[R02] 变量赋值与使用
来源：http://read.share.zdbjq.cn/Article/details/gphfpefcg.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fehbvm.com/Article/details/gpzdqvwnb.sHtML

[R03] 只读变量
来源：http://baike.zdbjq.cn/Article/details/glyykzzsj.sHtML

readonly PI=3.14
来源：http://www.blog.hesvh.cn/Article/details/gmoztlhjf.sHtML

[R04] 位置参数
来源：http://read.share.hesvh.cn/Article/details/ghtmcsygg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fehbvm.com/Article/details/gyjkldypi.sHtML

[R05] 参数默认值
来源：http://www.m.share.hesvh.cn/Article/details/ggrvftljm.sHtML

name="${1:-default}"
来源：http://baike.zdbjq.cn/Article/details/gcxdqfsua.sHtML

[R06] 判断命令是否存在
来源：http://m.share.zdbjq.cn/Article/details/gcuqsawao.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gkmubckub.sHtML

[R07] if 判断文件
来源：http://www.blog.zdbjq.cn/Article/details/ghauxrlpx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.zdbjq.cn/Article/details/gmfzidjxp.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/gxqqfpatk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.hesvh.cn/Article/details/gllxkkdck.sHtML

[R09] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gsmndegqg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.hesvh.cn/Article/details/gapuxsofp.sHtML

[R10] 正则匹配
来源：http://www.blog.fehbvm.com/Article/details/gtxxmxplq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/gaaytpojl.sHtML

[R11] case 多分支
来源：http://www.share.fehbvm.com/Article/details/gsvpddtrz.sHtML

case "$1" in
来源：http://mobile.fehbvm.com/Article/details/gmumfhpef.sHtML

start) echo "启动" ;;
来源：http://read.share.hesvh.cn/Article/details/gelmtiuhv.sHtML

stop)  echo "停止" ;;
来源：http://wap.hesvh.cn/Article/details/gemehphrk.sHtML

*)     echo "未知命令" ;;
来源：http://baike.hesvh.cn/Article/details/gxqggburd.sHtML

esac
来源：http://read.share.zdbjq.cn/Article/details/geuhqecnb.sHtML

[R12] for 遍历文件
来源：http://wap.zdbjq.cn/Article/details/gbcvjquhy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fehbvm.com/Article/details/ghacgfudr.sHtML

[R13] for 计数循环
来源：http://mobile.hesvh.cn/Article/details/gavukcnsc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gkgpmaddw.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/glyhqutnu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/ghmturklp.sHtML

[R15] while 逐行读文件
来源：http://wap.fehbvm.com/Article/details/gortnymin.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.hesvh.cn/Article/details/gwipwehhs.sHtML

[R16] until 等待条件
来源：http://blog.zdbjq.cn/Article/details/gyaneebxi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gymqmzlel.sHtML

[R17] 数组定义与取值
来源：http://www.share.hesvh.cn/Article/details/gvniwortk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.zdbjq.cn/Article/details/gwwaaybrw.sHtML

[R18] 遍历数组
来源：http://wap.fehbvm.com/Article/details/gqpvfqhjw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fehbvm.com/Article/details/gjnehzssu.sHtML

[R19] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gomuaqqls.sHtML

echo "${#arr[@]}"
来源：http://wap.fehbvm.com/Article/details/gxswfygvx.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fehbvm.com/Article/details/ggcpkelre.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.zdbjq.cn/Article/details/gksauhiao.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/glgyazgrt.sHtML

echo "${#s}"
来源：http://blog.hesvh.cn/Article/details/glizffnlg.sHtML

[R22] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gwltzqtnx.sHtML

echo "${s:0:5}"
来源：http://wap.hesvh.cn/Article/details/gzxxzsuvu.sHtML

[R23] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/glqcxmnau.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.zdbjq.cn/Article/details/grqznbcdr.sHtML

[R24] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gigdlfhux.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.hesvh.cn/Article/details/ggchneopz.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.zdbjq.cn/Article/details/gcizrpdxy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.hesvh.cn/Article/details/gdannfeng.sHtML

[R26] 命令替换
来源：http://wap.zdbjq.cn/Article/details/gnyhwvtex.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fehbvm.com/Article/details/gkbakrxvt.sHtML

[R27] 算术展开
来源：http://m.share.fehbvm.com/Article/details/gxrdxgqbl.sHtML

echo $((1 + 2 * 3))
来源：http://3g.hesvh.cn/Article/details/gciqbxxsr.sHtML

[R28] 浮点运算
来源：http://m.share.fehbvm.com/Article/details/gyspsqkxv.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.hesvh.cn/Article/details/gxnbtglve.sHtML

[R29] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gqtnxmlsz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.zdbjq.cn/Article/details/gjqeghhnk.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fehbvm.com/Article/details/gtjlzkafh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.hesvh.cn/Article/details/ggiizbnwo.sHtML

[R31] 局部变量
来源：http://baike.fehbvm.com/Article/details/gdmnccpxo.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fehbvm.com/Article/details/gqxuqccba.sHtML

[R32] 参数个数校验
来源：http://m.share.fehbvm.com/Article/details/gaydgxcwn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gwkhahgje.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/gedybztyj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.zdbjq.cn/Article/details/gwhebexkk.sHtML

[R34] 退出时清理
来源：http://blog.zdbjq.cn/Article/details/gbfqdvxss.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gregpszbq.sHtML

[R35] 后台执行并等待
来源：http://www.share.zdbjq.cn/Article/details/gdbxllnrn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fehbvm.com/Article/details/gcqufuako.sHtML

[R36] 并发执行多个任务
来源：http://m.share.zdbjq.cn/Article/details/gqgddwezd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.zdbjq.cn/Article/details/gpxbqvtqn.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fehbvm.com/Article/details/gjetbynuu.sHtML

files=$(ls -1)
来源：http://baike.hesvh.cn/Article/details/gwdgozhwa.sHtML

[R38] 管道串联
来源：http://blog.fehbvm.com/Article/details/gisglaeqt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fehbvm.com/Article/details/gyishmgmk.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.hesvh.cn/Article/details/gpldzeftg.sHtML

cmd > out.log 2>&1
来源：http://m.share.fehbvm.com/Article/details/grgrkpmcx.sHtML

[R40] 追加写日志
来源：http://mobile.fehbvm.com/Article/details/gbzjkwvjl.sHtML

echo "log" >> out.log
来源：http://wap.hesvh.cn/Article/details/gtrcmcgbb.sHtML

[R41] 丢弃输出
来源：http://read.share.zdbjq.cn/Article/details/ghldkqnwg.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gwgmwrvld.sHtML

[R42] 输入重定向
来源：http://read.share.hesvh.cn/Article/details/gfoyrcbtz.sHtML

wc -l < a.txt
来源：http://m.share.fehbvm.com/Article/details/grxvmmijh.sHtML

[R43] 按名字查找文件
来源：http://baike.zdbjq.cn/Article/details/ghpfmuiuc.sHtML

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/gpbvlexea.sHtML

[R44] 按修改时间查找
来源：http://www.blog.hesvh.cn/Article/details/galdgbysv.sHtML

find . -mtime -7 -type f
来源：http://m.share.zdbjq.cn/Article/details/gbyxdbtqq.sHtML

[R45] 批量删除
来源：http://m.share.fehbvm.com/Article/details/gxddimssv.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.hesvh.cn/Article/details/guuhokcfg.sHtML

[R46] 递归替换文件内容
来源：http://baike.fehbvm.com/Article/details/gnakqbhqk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fehbvm.com/Article/details/goijqhjcu.sHtML

[R47] sed 单行替换
来源：http://mobile.hesvh.cn/Article/details/gzxypsuce.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gaoucbiuu.sHtML

[R48] awk 取指定列
来源：http://wap.fehbvm.com/Article/details/gsxtoflrn.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fehbvm.com/Article/details/gzfvszomr.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/gkvugktyw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.hesvh.cn/Article/details/gadpkpmyv.sHtML

[R50] awk 求和
来源：http://m.share.hesvh.cn/Article/details/gjgzzjbzi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gjdwdlfnh.sHtML

[R51] 排序去重取前几
来源：http://baike.hesvh.cn/Article/details/gycbplssu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.zdbjq.cn/Article/details/gtkuvtkxk.sHtML

[R52] 统计行数
来源：http://m.share.hesvh.cn/Article/details/gyksyatus.sHtML

wc -l a.txt
来源：http://mobile.hesvh.cn/Article/details/gywaqmkjn.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.hesvh.cn/Article/details/gybwyusvd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.zdbjq.cn/Article/details/gljvkhhes.sHtML

[R54] 比较两个文件
来源：http://www.share.zdbjq.cn/Article/details/glqeetqch.sHtML

diff a.txt b.txt
来源：http://m.share.zdbjq.cn/Article/details/gblfscimm.sHtML

[R55] 压缩与解压
来源：http://blog.fehbvm.com/Article/details/gaagwpsjx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fehbvm.com/Article/details/gmqbxdnbx.sHtML

[R56] 远程拷贝
来源：http://3g.hesvh.cn/Article/details/gdgyjqgor.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/gowtvdxog.sHtML

[R57] 远程执行命令
来源：http://baike.hesvh.cn/Article/details/ghzilgimk.sHtML

ssh user@host 'uptime'
来源：http://mobile.zdbjq.cn/Article/details/gidipfrnr.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/gfiytzike.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.zdbjq.cn/Article/details/ggggaedfn.sHtML

[R59] 发 POST JSON
来源：http://3g.zdbjq.cn/Article/details/geckbzxgm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/gqpjneoqd.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gysfowixo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fehbvm.com/Article/details/gjhhbvnin.sHtML

[R61] 磁盘占用
来源：http://www.share.fehbvm.com/Article/details/gvgkntymt.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/guvmmbghh.sHtML

[R62] 找最占空间的文件
来源：http://mobile.hesvh.cn/Article/details/gxksflhva.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fehbvm.com/Article/details/gdpslegjr.sHtML

[R63] 内存与进程
来源：http://read.share.fehbvm.com/Article/details/gluhlmvnn.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fehbvm.com/Article/details/gsleyrnwc.sHtML

[R64] 结束进程
来源：http://www.share.fehbvm.com/Article/details/gfkgucaoe.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.zdbjq.cn/Article/details/gakrfthbn.sHtML

[R65] 查看端口占用
来源：http://read.share.hesvh.cn/Article/details/gzlxwcgsd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.hesvh.cn/Article/details/gscnpqdad.sHtML

[R66] 定时任务
来源：http://read.share.fehbvm.com/Article/details/gnsjqdoxj.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/gzbomzohy.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.hesvh.cn/Article/details/gftxjilye.sHtML

openssl rand -hex 16
来源：http://blog.hesvh.cn/Article/details/gqeqgdgsh.sHtML

[R68] 计算文件校验值
来源：http://www.share.fehbvm.com/Article/details/gfxwgoknc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.zdbjq.cn/Article/details/gjwudefqk.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fehbvm.com/Article/details/gudlksofo.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.zdbjq.cn/Article/details/ghhsaszuf.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/gcsmkdlzh.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fehbvm.com/Article/details/gsjavleds.sHtML

[R71] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/getguwqpg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fehbvm.com/Article/details/goletgtgh.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/gkrydthal.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gozcvgvuv.sHtML

[R73] 分割大日志
来源：http://read.share.hesvh.cn/Article/details/gexqfmtfl.sHtML

split -l 1000 big.log part_
来源：http://www.share.fehbvm.com/Article/details/gfxnqvjnf.sHtML

[R74] 批量重命名
来源：http://baike.fehbvm.com/Article/details/gkmdomjfm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/gnldkjrzg.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/gvnzthgoi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/gyiqrjufp.sHtML

[R76] 使用临时文件
来源：http://read.share.zdbjq.cn/Article/details/gamquehgz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/ggjtywriu.sHtML

[R77] 读取用户输入
来源：http://m.share.zdbjq.cn/Article/details/garromoks.sHtML

read -rp "请输入: " ans
来源：http://3g.fehbvm.com/Article/details/gwblmeqin.sHtML

[R78] 交互式菜单
来源：http://www.blog.fehbvm.com/Article/details/gbntingxi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fehbvm.com/Article/details/gbvavkzvz.sHtML

[R79] 解析命令行选项
来源：http://www.share.fehbvm.com/Article/details/gjyjamfqa.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fehbvm.com/Article/details/gtzynundv.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.zdbjq.cn/Article/details/gjdjlazim.sHtML

time ./run.sh
来源：http://baike.fehbvm.com/Article/details/guemstmio.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gsrmmzwbr.sHtML

S. C / C++ 专题
来源：http://baike.hesvh.cn/Article/details/gnfbcsyzz.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwizzjlkk.sHtML

[S01] C：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gfrxcphwk.sHtML

#include <stdio.h>
来源：http://blog.hesvh.cn/Article/details/gsdrclesw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.zdbjq.cn/Article/details/gagazlumg.sHtML

[S02] C：变量与格式化输出
来源：http://wap.hesvh.cn/Article/details/gguevswlw.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fehbvm.com/Article/details/gyvtmmurk.sHtML

[S03] C：读入整数
来源：http://www.blog.zdbjq.cn/Article/details/gcopsazbx.sHtML

int x; scanf("%d", &x);
来源：http://blog.fehbvm.com/Article/details/gzewhviis.sHtML

[S04] C：字符串复制
来源：http://read.share.fehbvm.com/Article/details/gzbraafca.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.hesvh.cn/Article/details/gkgbucaha.sHtML

[S05] C：字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gzjznanlp.sHtML

strlen(s)
来源：http://blog.hesvh.cn/Article/details/gwqvlbkwj.sHtML

[S06] C：字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gzwrzizla.sHtML

strcmp(a, b) == 0
来源：http://baike.fehbvm.com/Article/details/glcogwuxy.sHtML

[S07] C：数组遍历求和
来源：http://m.share.hesvh.cn/Article/details/gixrgyvre.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.zdbjq.cn/Article/details/gyxkycsnk.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.zdbjq.cn/Article/details/ggttfcets.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.zdbjq.cn/Article/details/gwjwhoque.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/gejjbpzhs.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fehbvm.com/Article/details/gpnakzczl.sHtML

[S10] C：指针与解引用
来源：http://blog.fehbvm.com/Article/details/gkgggcqwr.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fehbvm.com/Article/details/gozohtizp.sHtML

[S11] C：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gczitvizp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.zdbjq.cn/Article/details/gjbywellw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.hesvh.cn/Article/details/gkxcpdwta.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/ggfxxexte.sHtML

[S12] C：写文件
来源：http://baike.fehbvm.com/Article/details/gptnucqqi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fehbvm.com/Article/details/glyhoxprz.sHtML

[S13] C：宏定义
来源：http://read.share.hesvh.cn/Article/details/gmcnwnukn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/glyhwisfr.sHtML

[S14] C：枚举
来源：http://blog.zdbjq.cn/Article/details/gkbkhwgeg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fehbvm.com/Article/details/gtsqonghc.sHtML

[S15] C：类型转换
来源：http://read.share.zdbjq.cn/Article/details/gfvdbdtus.sHtML

(double) a / b
来源：http://m.share.fehbvm.com/Article/details/ggoedjqny.sHtML

[S16] C：位操作置位
来源：http://mobile.fehbvm.com/Article/details/giesqakrb.sHtML

x |= (1 << 3);
来源：http://mobile.hesvh.cn/Article/details/gqqfqhtxd.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fehbvm.com/Article/details/gnehovdyd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.zdbjq.cn/Article/details/gheubrngg.sHtML

[S18] C：命令行参数
来源：http://3g.hesvh.cn/Article/details/gfengakbl.sHtML

int main(int argc, char **argv)
来源：http://www.blog.hesvh.cn/Article/details/gffokgcuy.sHtML

[S19] C：快速排序
来源：http://m.share.zdbjq.cn/Article/details/grmlykogz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gekxktqhb.sHtML

[S20] C：二分查找
来源：http://baike.hesvh.cn/Article/details/gsamcseny.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/grxwrkluk.sHtML

[S21] C：字符类别判断
来源：http://blog.fehbvm.com/Article/details/glnbhfhem.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.zdbjq.cn/Article/details/gibtvkpaz.sHtML

[S22] C：字符串转数字
来源：http://baike.zdbjq.cn/Article/details/gufdlkgoh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fehbvm.com/Article/details/gihnziisq.sHtML

[S23] C：随机数
来源：http://m.share.hesvh.cn/Article/details/gzdzovigm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.zdbjq.cn/Article/details/gperiukgm.sHtML

[S24] C：获取本地时间
来源：http://baike.fehbvm.com/Article/details/gezlcjzlw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fehbvm.com/Article/details/gbqxexmiz.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/gvrwhcaal.sHtML

memcpy(dst, src, n);
来源：http://mobile.zdbjq.cn/Article/details/ghdekatkk.sHtML

[S26] C：内存清零
来源：http://www.share.zdbjq.cn/Article/details/gosmvukgl.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.hesvh.cn/Article/details/guanmpgmj.sHtML

[S27] C：定义常量
来源：http://read.share.fehbvm.com/Article/details/glyevyypr.sHtML

const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/ghyavlndg.sHtML

[S28] C：静态变量
来源：http://www.blog.zdbjq.cn/Article/details/gwquadfik.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/glianilka.sHtML

[S29] C：变参函数
来源：http://www.share.zdbjq.cn/Article/details/gbrhqobmu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/gchmlrzqj.sHtML

[S30] C：头文件保护
来源：http://blog.hesvh.cn/Article/details/gobrowbzs.sHtML

#ifndef X_H
来源：http://read.share.fehbvm.com/Article/details/gmdifvnfe.sHtML

#define X_H
来源：http://www.m.share.hesvh.cn/Article/details/gbxbdvnti.sHtML

#endif
来源：http://baike.hesvh.cn/Article/details/ggidbowub.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gcqttiyjn.sHtML

#include <iostream>
来源：http://www.blog.fehbvm.com/Article/details/gzzytiblv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.zdbjq.cn/Article/details/gpnewpnbf.sHtML

[S32] C++：字符串
来源：http://blog.hesvh.cn/Article/details/grrssjqcw.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.hesvh.cn/Article/details/ghrgcfvzg.sHtML

[S33] C++：vector 增删
来源：http://www.share.fehbvm.com/Article/details/gvmnxoddy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.zdbjq.cn/Article/details/ggcweqkwk.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/gscccbgoc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fehbvm.com/Article/details/gewduorbs.sHtML

[S35] C++：map
来源：http://www.share.fehbvm.com/Article/details/gtsllkcby.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/ghlsjtkgg.sHtML

[S36] C++：unordered_map
来源：http://3g.hesvh.cn/Article/details/gpttpzmqz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gezhasalt.sHtML

[S37] C++：set
来源：http://m.share.zdbjq.cn/Article/details/ggftsyzne.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.zdbjq.cn/Article/details/gvdwubldi.sHtML

[S38] C++：排序
来源：http://www.share.hesvh.cn/Article/details/gabwftckl.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.hesvh.cn/Article/details/gqbqavubw.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fehbvm.com/Article/details/gfydpivgx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.zdbjq.cn/Article/details/gnngizukf.sHtML

[S40] C++：查找元素
来源：http://baike.zdbjq.cn/Article/details/gfchusxxt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fehbvm.com/Article/details/gkhcjtafs.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fehbvm.com/Article/details/godhfklfc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.zdbjq.cn/Article/details/glzvlmsbp.sHtML

[S42] C++：继承与虚函数
来源：http://blog.hesvh.cn/Article/details/gcsfuxayi.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/gphzugelt.sHtML

[S43] C++：智能指针
来源：http://wap.hesvh.cn/Article/details/gdwhwloyx.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/gryfhrfsu.sHtML

[S44] C++：引用传参
来源：http://mobile.hesvh.cn/Article/details/gvznwnnvy.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.hesvh.cn/Article/details/gjbuxopih.sHtML

[S45] C++：lambda
来源：http://3g.zdbjq.cn/Article/details/gxydfsnhf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.zdbjq.cn/Article/details/gplhkezzn.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/gucynwgxm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.zdbjq.cn/Article/details/gcwtuxkwp.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fehbvm.com/Article/details/gnrajgfed.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.zdbjq.cn/Article/details/gdrjsshpd.sHtML

[S48] C++：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gcqwkyfjv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fehbvm.com/Article/details/ghlknmjwf.sHtML

while (std::getline(in, line)) { }
来源：http://baike.zdbjq.cn/Article/details/gqzlzmuxx.sHtML

[S49] C++：写文件
来源：http://baike.hesvh.cn/Article/details/ggunhpspd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.hesvh.cn/Article/details/gbgdvdwzx.sHtML

[S50] C++：格式化数字
来源：http://wap.fehbvm.com/Article/details/gxfrblalj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.hesvh.cn/Article/details/gnkdxtown.sHtML

[S51] C++：显式类型转换
来源：http://m.share.hesvh.cn/Article/details/grualoqua.sHtML

static_cast<double>(a) / b
来源：http://read.share.zdbjq.cn/Article/details/glwwfjshm.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.hesvh.cn/Article/details/gqepcjinl.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.zdbjq.cn/Article/details/gxghqeoqp.sHtML

[S53] C++：移动语义
来源：http://m.share.zdbjq.cn/Article/details/gplcjuhea.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.hesvh.cn/Article/details/gashgcmyz.sHtML

[S54] C++：异常处理
来源：http://wap.zdbjq.cn/Article/details/gjlzeuevh.sHtML


<!-- 参考信息 -->